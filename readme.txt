## Qrio.js
Javascript library that adds QR/bar code scanning and QR code generation capabilities to web pages.

Demo: https://gregsidal.github.io/qrio/

To use with default behaviour (popovers, see demo):

Include qrio.css, qrcode.js, and qrio.js, and place at bottom of HTML:
  <div id="qrio-generator-html"></div> 
  <div id="qrio-reader-html"></div>

During page init (onload or onDOMContentLoaded) call:
  QRIO.generator.insertHTML();
  QRIO.reader.insertHTML();
   
To generate and display a QR code (simplest use, takes message from span):
  <span onclick="QRIO.generator.open( this );">Hello, world, let's get this encoded.</span>
   
To scan QR and/or bar codes (simplest use, places result in span):
  <span onclick="QRIO.reader.open( this );">Click here to scan a QR/bar code.</span>

See comments in Qrio.js for more.  See QRIO.generator.HTML and QRIO.reader.HTML for default HTML; see qrio.css for default css

Scanning uses the newer BarcodeDetector javascript API.
