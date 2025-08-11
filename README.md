<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Security Risk Demonstration – oneupfitness.ca</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      color: #333;
    }

    header {
      padding: 20px;
      background-color: #b30000;
      color: red;
      text-align: center;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    }

    h2 {
      margin: 0 0 10px;
    }

    .notice {
      background: #fff3cd;
      color: #856404;
      border: 1px solid #ffeeba;
      padding: 12px;
      margin: 20px auto;
      width: 90%;
      max-width: 800px;
      font-size: 15px;
      border-radius: 6px;
    }

    iframe {
      display: block;
      width: 100%;
      height: 90vh;
      border: none;
      margin-top: 10px;
      box-shadow: 0 0 15px rgba(0,0,0,0.2);
    }
  </style>
</head>
<body>
  <header>
    <h2>⚠ Security Alert: Unauthorized Embedding Detected</h2>
    <p>This is a clickjacking vulnerability demonstration for <strong>southlandfisheries.com</strong></p>
  </header>

  <div class="notice">
    <strong>Context:</strong> The following external website (<code>southlandfisheries.com</code>) has been embedded here without any permission, and without implementing standard security headers such as <code>X-Frame-Options</code> or <code>Content-Security-Policy: frame-ancestors</code>.
    <br><br>
    This indicates the site is vulnerable to <em>clickjacking</em> attacks — where attackers can trick users into interacting with hidden elements on the real site (e.g. buttons, logins) while believing they’re on a safe page.
    <br><br>
    Developers and site owners are strongly advised to implement frame-busting protections immediately.
  </div>

  <!-- IFRAME DEMONSTRATING THE VULNERABILITY -->
  <iframe src="http://southlandfisheries.com
"></iframe>
</body>
</html>
