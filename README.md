# aceitaFacil HTML + jQuery Example

Use this example to easily charge customers using aceitaFacil functions.

## Installation

1. Obtain the latest version of the aceitaFacil HTML + jQuery Example with:

    ```sh
    git clone https://github.com/aceitaFacil/HTML-jQuery-Example
    ```

2. Generate a base64 string of your public key concatenated with a colon:

    1. Open the developer tools console from your browser (instructions for
       [Chrome][devtools-chrome] and [Firefox][devtools-firefox]).

    2. Type `btoa('INSERT YOUR PUBLIC KEY HERE' + ':');`.

    3. Take note of the generated string.

3. Change the `Authorization` header to include the base64 string generated
   above:

    ```javascript
    headers: { 'Authorization': 'Basic SW5zZXJ0IHlvdXIgcHVibGljIGtleSBoZXJlOg==' },
    ```

4. Update the path to your server-side script:

    ```html
    <form id="frmPayment" action="https://YOUR_SITE/path/to/payment" method="post">
    ```

## Documentation

* Please see https://aceitaFacil.com/docs for up-to-date documentation.

[devtools-chrome]: https://developer.chrome.com/devtools/docs/shortcuts
[devtools-firefox]: https://developer.mozilla.org/en-US/docs/Tools/Keyboard_shortcuts
