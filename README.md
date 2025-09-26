<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1.0">
  <title>Subscribe to Sir Dennis's Updates</title>
  <style>
    body { font-family: 'Segoe UI', Arial, sans-serif; background: #f6f8fa; padding: 40px; }
    .fs-form { max-width: 540px; margin: auto; background: #fff; padding: 30px 28px 24px 28px; border-radius: 10px; box-shadow: 0 6px 24px rgba(0,0,0,0.10); }
    .fs-label { display: block; margin-top: 18px; margin-bottom: 6px; font-weight: 500; }
    .fs-input, .fs-select { width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 4px; font-size: 16px; }
    .fs-checkbox-group { margin-top: 6px; display: flex; flex-wrap: wrap; gap: 18px; }
    .fs-checkbox-field { display: flex; align-items: center; }
    .fs-checkbox-wrapper { margin-right: 6px; }
    .fs-button-group { margin-top: 24px; }
    .fs-button { background: #0366d6; color: #fff; border: none; padding: 12px 0; width: 100%; border-radius: 4px; font-size: 18px; cursor: pointer; }
    .fs-button:hover { background: #024eaf; }
    .footer { margin-top: 24px; text-align: center; color: #aaa; font-size: 12px; }
    .message { margin-top: 18px; font-size: 16px; text-align: center; }
    .message.success { color: #007b3c; }
    .message.error { color: #c00; }
    .fs-upload-note { font-size: 13px; color: #555; margin-top: 3px; }
    @media (max-width: 600px) { .fs-form { padding: 14px; } }
  </style>
</head>
<body>
  <form
    id="signup-form"
    action="https://supabase.com/nmqerswvdrbphkawjwmv" <!-- replace with your Formspree form ID if different -->
    class="fs-form"
    target="_top"
    method="POST"
    enctype="multipart/form-data"
    autocomplete="off"
  >
    <h2>Subscribe to Updates</h2>

    <div class="fs-field">
      <label class="fs-label" for="full-name">Full Name</label>
      <input class="fs-input" id="full-name" name="full-name" placeholder="Enter your name (optional)" autocomplete="name" />
    </div>

    <div class="fs-field">
      <label class="fs-label" for="email-address">Email Address</label>
      <input class="fs-input" id="email-address" name="email-address" placeholder="Enter your email address" required type="email" autocomplete="email" />
    </div>

    <div class="fs-field">
      <label class="fs-label" for="phone-number">Phone Number</label>
      <input class="fs-input" id="phone-number" name="phone-number" type="tel" placeholder="Enter your phone number" pattern="[0-9+\-\s]{7,20}" autocomplete="tel" required />
    </div>

    <div class="fs-field">
      <label class="fs-label" for="password">Password</label>
      <input class="fs-input" id="password" name="password" type="password" placeholder="Password" minlength="6" required autocomplete="new-password" />
    </div>

    <div class="fs-field">
      <label class="fs-label" for="confirm-password">Confirm Password</label>
      <input class="fs-input" id="confirm-password" name="confirm-password" type="password" placeholder="Re-enter Password" minlength="6" required autocomplete="new-password" />
    </div>

    <div class="fs-field">
      <label class="fs-label" for="company-name">Company Name</label>
      <input class="fs-input" id="company-name" name="company-name" placeholder="Enter your company (optional)" />
    </div>

    <div class="fs-field">
      <label class="fs-label" for="job-title">Job Title</label>
      <input class="fs-input" id="job-title" name="job-title" placeholder="Enter your job title (optional)" />
    </div>

    <div class="fs-field">
      <label class="fs-label">Topics of Interest</label>
      <div class="fs-checkbox-group">
        <div class="fs-checkbox-field">
          <div class="fs-checkbox-wrapper">
            <input class="fs-checkbox" id="topics-of-interest-product-updates" name="topics-of-interest" type="checkbox" value="product-updates" />
          </div>
          <div><label class="fs-label" for="topics-of-interest-product-updates">Product Updates</label></div>
        </div>
        <div class="fs-checkbox-field">
          <div class="fs-checkbox-wrapper">
            <input class="fs-checkbox" id="topics-of-interest-blog-posts" name="topics-of-interest" type="checkbox" value="blog-posts" />
          </div>
          <div><label class="fs-label" for="topics-of-interest-blog-posts">Blog Posts</label></div>
        </div>
        <div class="fs-checkbox-field">
          <div class="fs-checkbox-wrapper">
            <input class="fs-checkbox" id="topics-of-interest-promotions" name="topics-of-interest" type="checkbox" value="promotions" />
          </div>
          <div><label class="fs-label" for="topics-of-interest-promotions">Promotions</label></div>
        </div>
        <div class="fs-checkbox-field">
          <div class="fs-checkbox-wrapper">
            <input class="fs-checkbox" id="topics-of-interest-events" name="topics-of-interest" type="checkbox" value="events" />
          </div>
          <div><label class="fs-label" for="topics-of-interest-events">Events</label></div>
        </div>
      </div>
    </div>

    <div class="fs-field">
      <label class="fs-label" for="email-frequency">Preferred Email Frequency</label>
      <select class="fs-select" id="email-frequency" name="email-frequency" required>
        <option value="">-- Select Frequency --</option>
        <option value="weekly">Weekly</option>
        <option value="monthly">Monthly</option>
        <option value="occasionally">Occasionally</option>
      </select>
    </div>

    <div class="fs-field">
      <label class="fs-label" for="referral-source">How Did You Hear About Us?</label>
      <input class="fs-input" id="referral-source" name="referral-source" placeholder="Let us know how you found us (optional)" />
    </div>

    <div class="fs-field">
      <label class="fs-label" for="profile-upload">Profile Photo / Document</label>
      <input class="fs-input" id="profile-upload" name="profile-upload" type="file" accept=".jpg,.jpeg,.png,.pdf,.doc,.docx" />
      <div class="fs-upload-note">Accepted: jpg, png, pdf, doc, docx. Max size: 2MB.</div>
    </div>

    <div class="fs-button-group"><button class="fs-button" type="submit">Subscribe</button></div>

    <div id="form-message" class="message" style="display:none;"></div>

    <div class="footer">
      &copy; 2025 Sir Dennis. Managed by tyadeola.<br>
      <strong>No affiliation with Facebook, Meta, or Mark Zuckerberg.</strong>
    </div>
  </form>

  <script>
    // Enhanced validation and Formspree submission
    document.getElementById('signup-form').addEventListener('submit', async function(e) {
      e.preventDefault();
      const form = e.target;
      const messageDiv = document.getElementById('form-message');
      messageDiv.style.display = "none";
      messageDiv.textContent = "";
      messageDiv.className = "message";

      // Password validation
      const pw = document.getElementById('password').value;
      const cpw = document.getElementById('confirm-password').value;
      if (pw.length < 6) {
        messageDiv.textContent = "Password must be at least 6 characters.";
        messageDiv.className += " error";
        messageDiv.style.display = "block";
        return;
      }
      if (pw !== cpw) {
        messageDiv.textContent = "Passwords do not match.";
        messageDiv.className += " error";
        messageDiv.style.display = "block";
        return;
      }

      // Email validation
      const email = document.getElementById('email-address').value;
      if (!/^[^@]+@[^@]+\\.[^@]+$/.test(email)) {
        messageDiv.textContent = "Invalid email address.";
        messageDiv.className += " error";
        messageDiv.style.display = "block";
        return;
      }

      // Phone number validation
      const phone = document.getElementById('phone-number').value;
      if (!/^[0-9+\\-\\s]{7,20}$/.test(phone)) {
        messageDiv.textContent = "Please enter a valid phone number (7-20 digits, numbers, spaces, + or -).";
        messageDiv.className += " error";
        messageDiv.style.display = "block";
        return;
      }

      // File validation
      const fileInput = document.getElementById('profile-upload');
      if (fileInput.files.length > 0) {
        const file = fileInput.files[0];
        const allowedTypes = ['image/jpeg', 'image/png', 'application/pdf', 'application/msword', 'application/vnd.openxmlformats-officedocument.wordprocessingml.document'];
        if (!allowedTypes.includes(file.type)) {
          messageDiv.textContent = "File type not allowed. Only jpg, png, pdf, doc, docx.";
          messageDiv.className += " error";
          messageDiv.style.display = "block";
          return;
        }
        if (file.size > 2 * 1024 * 1024) {
          messageDiv.textContent = "File too large. Max size is 2MB.";
          messageDiv.className += " error";
          messageDiv.style.display = "block";
          return;
        }
      }

      // Formspree submission
      const data = new FormData(form);
      try {
        const response = await fetch(form.getAttribute('action'), {
          method: 'POST',
          body: data,
          headers: { 'Accept': 'application/json' }
        });
        if (response.ok) {
          messageDiv.textContent = "Thank you for subscribing! Your details have been received.";
          messageDiv.className = "message success";
          messageDiv.style.display = "block";
          form.reset();
        } else {
          const result = await response.json();
          messageDiv.textContent = (result.errors && result.errors[0].message) || "Oops! There was a problem submitting your form.";
          messageDiv.className = "message error";
          messageDiv.style.display = "block";
        }
      } catch (error) {
        messageDiv.textContent = "Network error. Please try again later.";
        messageDiv.className = "message error";
        messageDiv.style.display = "block";
      }
    });
  </script>
</body>
</html>
