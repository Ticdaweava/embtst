<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Clickjacking Proof-of-Concept</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background: #f9f9f9;
    padding: 20px;
  }
  h1 {
    color: #b00000;
  }
  .iframe-container {
    position: relative;
    width: 100%;
    max-width: 1024px;
    height: 600px;
    border: 3px solid #b00000;
    overflow: hidden;
  }
  iframe {
    width: 100%;
    height: 100%;
    border: none;
  }
  /* Example overlay to simulate malicious intent */
  .overlay {
    position: absolute;
    top: 50px;
    left: 50px;
    width: 200px;
    height: 100px;
    background: rgba(255, 0, 0, 0.4);
    z-index: 2;
    pointer-events: none; /* allows clicks to pass through */
  }
</style>
</head>
<body>
  <h1>⚠ Security Demonstration: Clickjacking Risk</h1>
  <p>This page shows how <strong>[Target Site]</strong> can be embedded without permission.
     A malicious actor could place invisible or misleading overlays to trick users into clicking
     something they didn’t intend.</p>

  <div class="iframe-container">
    <div class="overlay">Malicious Overlay Example</div>
    <iframe src="https://southlandfisheries.com"></iframe>
  </div>

  <p><strong>Recommendation:</strong> Add security headers to prevent this:
    <code>X-Frame-Options: SAMEORIGIN</code> or
    <code>Content-Security-Policy: frame-ancestors 'self'</code>.
  </p>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Clickjacking Proof-of-Concept</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background: #f9f9f9;
    padding: 20px;
  }
  h1 {
    color: #b00000;
  }
  .iframe-container {
    position: relative;
    width: 100%;
    max-width: 1024px;
    height: 600px;
    border: 3px solid #b00000;
    overflow: hidden;
  }
  iframe {
    width: 100%;
    height: 100%;
    border: none;
  }
  /* Example overlay to simulate malicious intent */
  .overlay {
    position: absolute;
    top: 50px;
    left: 50px;
    width: 200px;
    height: 100px;
    background: rgba(255, 0, 0, 0.4);
    z-index: 2;
    pointer-events: none; /* allows clicks to pass through */
  }
</style>
</head>
<body>
  <h1>⚠ Security Demonstration: Clickjacking Risk</h1>
  <p>This page shows how <strong>[Target Site]</strong> can be embedded without permission.
     A malicious actor could place invisible or misleading overlays to trick users into clicking
     something they didn’t intend.</p>

  <div class="iframe-container">
    <div class="overlay">Malicious Overlay Example</div>
    <iframe src="https://southlandfisheries.com"></iframe>
  </div>

  <p><strong>Recommendation:</strong> Add security headers to prevent this:
    <code>X-Frame-Options: SAMEORIGIN</code> or
    <code>Content-Security-Policy: frame-ancestors 'self'</code>.
  </p>
</body>
</html>
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Clickjacking Proof</title>
<style>
  body {
    font-family: Arial, sans-serif;
    background: #fafafa;
    margin: 20px;
  }
  .iframe-box {
    position: relative;
    width: 100%;
    max-width: 1024px;
    height: 600px;
    border: 2px solid red;
  }
  iframe {
    width: 100%;
    height: 100%;
    border: none;
  }
  .overlay {
    position: absolute;
    top: 80px;
    left: 100px;
    width: 200px;
    height: 100px;
    background: rgba(255, 0, 0, 0.3);
    z-index: 2;
    pointer-events: none;
    font-weight: bold;
    text-align: center;
    padding-top: 35px;
    color: white;
  }
</style>
</head>
<body>

<h2>⚠ Clickjacking Demonstration</h2>
<p>This shows how <strong>southlandfisheries.com</strong> can be embedded without restriction.
A malicious site could place invisible overlays to trick users into clicking unintended areas.</p>

<div class="iframe-box">
  <div class="overlay">Fake Button</div>
  <iframe src="https://southlandfisheries.com"></iframe>
</div>

<p><strong>Fix:</strong> Add <code>X-Frame-Options: SAMEORIGIN</code> or
<code>Content-Security-Policy: frame-ancestors 'self'</code>.</p>

</body>
</html>
