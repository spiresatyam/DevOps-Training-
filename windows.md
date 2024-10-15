<!DOCTYPE html>
<html>
<head>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.6/clipboard.min.js"></script>
    <style>
        .copy-btn {
            cursor: pointer;
            margin-left: 5px;
            font-size: small;
        }
    </style>
</head>
<body>
    <h3>WindowsTools</h3>

    <pre><code id="code1">choco install virtualbox --version=7.0.8 -y</code><button class="copy-btn" data-clipboard-target="#code1">Copy</button></pre>
    <pre><code id="code2">choco install vagrant --version=2.2.3.7 -y</code><button class="copy-btn" data-clipboard-target="#code2">Copy</button></pre>
    <pre><code id="code3">choco install git -y</code><button class="copy-btn" data-clipboard-target="#code3">Copy</button></pre>

    <script>
        var clipboard = new ClipboardJS('.copy-btn');
        clipboard.on('success', function(e) {
            console.log('Copied:', e.text);
        });
        clipboard.on('error', function(e) {
            console.log('Copy failed');
        });
    </script>
</body>
</html>
