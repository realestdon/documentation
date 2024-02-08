======
Stripe
======

`Stripe <https://stripe.com/>`_ is a United States-based online payment solution provider allowing
businesses to accept **credit cards** and other payment methods.

Create your Stripe account with Odoo
====================================

The method to acquire your credentials depends on your hosting type:

.. tabs::
   .. group-tab:: Odoo Online

      #. :ref:`Navigate to the payment provider Stripe <payment_providers/supported_providers>` and
         click :guilabel:`Connect Stripe`.
      #. Go through the setup process and confirm your email address when Stripe sends you a
         confirmation email.
      #. At the end of the process, click :guilabel:`Agree and submit`. If all requested information
         has been submitted, you are then redirected to Odoo, and your payment provider is enabled.
      #. :ref:`stripe/local-payment-methods`.

   .. group-tab:: Odoo.sh or On-premise

      #. :ref:`Navigate to the payment provider Stripe <payment_providers/supported_providers>` and
         click :guilabel:`Connect Stripe`.
      #. Go through the setup process and confirm your email address when Stripe sends you a
         confirmation email.
      #. At the end of the process, click :guilabel:`Agree and submit`; you are then redirected to
         the payment provider **Stripe** in Odoo.
      #. :ref:`Fill in your credentials <stripe/api_keys>`.
      #. :ref:`Generate a webhook <stripe/webhook>`.
      #. Select a :ref:`payment journal <payment_providers/journal>`.
      #. Set the :guilabel:`State` field to :guilabel:`Enabled`.
      #. :ref:`stripe/local-payment-methods`.

.. tip::
   - To use an existing Stripe account, :ref:`activate the Developer mode <developer-mode>` and
     :ref:`enable Stripe manually <payment_providers/add_new>`. You can then :ref:`Fill in your
     credentials <stripe/api_keys>`, :ref:`generate a webhook <stripe/webhook>`, and enable the
     payment provider.
   - You can also test Stripe using the :ref:`payment_providers/test-mode`. To do so, first,
     `log into your Stripe dashboard <https://dashboard.stripe.com/dashboard>`_ and switch to the
     **Test mode**. Then, in Odoo, :ref:`activate the Developer mode <developer-mode>`,
     :ref:`navigate to the payment provider Stripe <payment_providers/supported_providers>`,
     :ref:`fill in your API credentials <stripe/api_keys>` with the test keys, and set the
     :guilabel:`State` field to :guilabel:`Test Mode`.

.. _stripe/api_keys:

Fill in your credentials
------------------------

If your **API credentials** are required to connect with your Stripe account, proceed as follows:

#. Go to `the API keys page on Stripe <https://dashboard.stripe.com/account/apikeys>`_, or log into
   your Stripe dashboard and go to :menuselection:`Developers --> API Keys`.
#. In the :guilabel:`Standard keys` section, copy the :guilabel:`Publishable key` and the
   :guilabel:`Secret key` and save them for later.
#. In Odoo, :ref:`navigate to the payment provider Stripe <payment_providers/supported_providers>`.
#. In the :guilabel:`Credentials` tab, fill in the :guilabel:`Publishable Key` and
   :guilabel:`Secret Key` fields with the values you previously saved.

.. _stripe/webhook:

Generate a webhook
------------------

If your **Webhook Signing Secret** is required to connect with your Stripe account, you can
create a webhook automatically or manually.

.. tabs::
   .. tab:: Create the webhook automatically

      Make sure your :ref:`Publishable and Secret keys <stripe/api_keys>` are filled in, then click
      :guilabel:`Generate your Webhook`.

   .. tab:: Create the webhook manually

      #. Go to the `Webhooks page on Stripe <https://dashboard.stripe.com/webhooks>`_, or log into
         your Stripe dashboard and go to :menuselection:`Developers --> Webhooks`.
      #. In the :guilabel:`Hosted endpoints` section, click :guilabel:`Add endpoint`. Then, in the
         :guilabel:`Endpoint URL` field, enter your Odoo database's URL, followed by
         `/payment/stripe/webhook`, e.g., `https://yourcompany.odoo.com/payment/stripe/webhook`.
      #.  Click :guilabel:`Select events` at the bottom of the form, then select the following
          events:

          - in the :guilabel:`Charge` section: :guilabel:`charge.refunded` and
            :guilabel:`charge.refund.updated`;
          - in the :guilabel:`Payment intent` section:
            :guilabel:`payment_intent.amount_capturable_updated`,
            :guilabel:`payment_intent.succeeded` and :guilabel:`payment_intent.payment_failed`;
          - in the :guilabel:`Setup intent` section: :guilabel:`setup_intent.succeeded`.

      #. Click :guilabel:`Add events`.
      #. Click :guilabel:`Add endpoint`, then click :guilabel:`Reveal` and save your
         :guilabel:`Signing secret` for later.
      #. In Odoo, :ref:`navigate to the payment provider Stripe
         <payment_providers/supported_providers>`.
      #. In the :guilabel:`Credentials` tab, fill the :guilabel:`Webhook Signing Secret` field with
         the value you previously saved.

      .. note::
         You can select other events, but they are currently not processed by Odoo.

.. _stripe/local-payment-methods:

Enable local payment methods
============================

Local payment methods are payment methods that are only available for specific providers and for
specific countries and currencies.

Odoo supports the following local payment methods for Stripe:

- Bancontact
- EPS
- giropay
- iDEAL
- Przelewy24 (P24)

To adapt the list of enabled payment methods, go to the :guilabel:`Configuration` tab and edit the
list of :guilabel:`Supported Payment Icons`.

.. note::
<<<<<<< HEAD
   - If a payment method record does not exist in the database and its related local payment method
     is listed above, it is considered enabled with Stripe.
||||||| parent of 6b472cb98 (temp)
   - If a payment icon record does not exist in the database and its related local payment method is
     listed above, it is considered enabled with Stripe.
=======
   - If a payment icon record does not exist in the database and its related local payment method is
     listed above, it is automatically enabled with Stripe.
>>>>>>> 6b472cb98 (temp)
   - If a local payment method is not listed above, it is not supported and cannot be enabled.

Enable Apple Pay
================

To allow customers to use the Apple Pay button to pay their eCommerce orders, go to the
:guilabel:`Configuration` tab, enable :guilabel:`Allow Express Checkout`, and click
:guilabel:`Enable Apple Pay`.

.. seealso::
   - :ref:`Express checkout and Google Pay <payment_providers/express_checkout>`
   - :doc:`../payment_providers`
   - :doc:`Use Stripe as a payment terminal in Point of Sale <../../sales/point_of_sale/payment_methods/terminals/stripe>`
