#$how Me The Money

Stripe is a payment processor that makes integration more simple.  Stripe sets itself apart from Paypal and Authorize.net by being a simplified and secure solution.  Don't confuse it with online shopping carts like Shopify or Big Cartel.  It simply lets you integrate with those, or your own shopping cart.

The major security feature it gives is that there is no need to save or be responsible for the credit card information entered on your site. PCI compliance for 1,000,000 e-commerce transactions is expected to be $100,000+ for compliance. Stripe takes care of that for you.  Awesome.

[Here is a link](https://memberful.com/blog/stripe-vs-paypal/) that talks about the differences between paypal and stripe including fees, security, and customer service.

## Basic Usage

Stripe can be accessed through their [API](https://stripe.com/docs/api), an included [Stripe.js](https://stripe.com/docs/stripe.js), and a pre-made [Checkout](https://stripe.com/checkout) solution.

For starters you'll need to setup and account[here](http://stripe.com) and use the .js include inside your body tag with this code to enable us to:

1) Collect credit card information with Stripe.js
2) Convert those details to what we call a single-use token
3) Send that token, with the rest of your form, to your server

```html
  <script type="text/javascript" src="https://js.stripe.com/v2/"></script>
  <script type="text/javascript">
  // This identifies your website in the createToken call below
  Stripe.setPublishableKey('YOUR KEY HERE');
</script>
```

Now setup your page with the information in your account.  Stripe does a good walk through [here](https://stripe.com/docs/stripe.js).


```js
var editor = new Editor();
editor.render();
```

The editor will take the position of the first `<textarea>` element. 

## Component

If you are using component, you can install it with:

    $ component install lepture/editor


## Seajs

If you are using seajs, you can install it with:

```
$ spm install lepture/editor
```

## Development

You can build the dist files with `grunt`. After this repo is cloned, dig into the repo, and install everything you need:

```
$ npm install
$ npm install grunt-cli -g
```

Now you can create the dist files:

```
$ grunt transport
```

You can get everything you need in the `build` directory.


## Configuration

The `Editor` Class accepts an option as the parameter. The supported options are:

* element (DOM)

  The element of the textarea. The default value is the first `<textarea>`.

* tools (array or false)

  If set false, the editor will have no toolbar.

* status (array or false)

  If set false, the editor will have no statusbar.

* actions (object)

* shortcuts (object)


## Contributing

Contribution is welcome. As a way to keep all code clean, we use Grunt to build our distributed files. Make sure you have read our [Contributing Guide](./CONTRIBUTING.md).

## License

Copyright (c) 2013 - 2014 by Hsiaoming Yang

Permission is hereby granted, free of charge to any noncommercial projects (paid for commercial support), including the rights to use, copy, modify, merge of the Software. Limitation of the rights to publish, distribute, and/or sell copies of the Software.

The above copyright notice and this permission notice shall be included in all copies of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

:10 [Demonstrate]: How to integrate stripe into your project
How to setup a Stripe account
How to use stripe to automatically build payment forms (Checkout)
How to use stripe.js to make custom checkout forms (custom payment form)
How to charge cards using node.js (https://stripe.com/docs/tutorials/charges)
:25 [Practice]: Create a project or group of test problems for the class to work on. This could be in the form of a few simple tasks or a larger, github-based project. You decide. The project/test problems should take about 20-25 minutes to complete.

:55 [Review]: questions, what did everyone learn, open discussion
