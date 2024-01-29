=======================
Start receiving tickets
=======================

Odoo *Helpdesk* offers multiple channels where customers can reach out for assistance, such as
email, live chat, and through a website's submission form. The variety of these contact options
provides customers with multiple opportunities to receive support quickly while also allowing the
support team to manage multi-channel support tickets from one central location.

Enable channel options to submit tickets
========================================

Go to :menuselection:`Helpdesk app --> Configuration --> Helpdesk Teams` and choose an existing
team, or click :guilabel:`New` to :doc:`create a new team <getting_started>`.

On the team's settings page, scroll down to the :guilabel:`Channels` and :guilabel:`Help Center`
sections. Enable one or more channels by checking the respective boxes.

- :ref:`Email Alias <receiving_tickets/email-alias>`
- :ref:`Live Chat <receiving_tickets/live-chat>`
- :ref:`Website Form <receiving_tickets/website-form>`

.. _receiving_tickets/email-alias:

Email Alias
-----------

The *Email Alias* setting creates tickets from messages sent to that team's specified email alias.

.. important::
   The following steps are for **Odoo Online** and **Odoo.sh** databases. For **On-premise**
   databases, external servers are required for email aliases.

When a new *Helpdesk* team is created, an email alias is created for it. This alias can be changed
on the team's settings page. To change a *Helpdesk* team's email alias, navigate to
:menuselection:`Helpdesk app --> Configuration --> Helpdesk Teams` and click on a team name to open
its settings page. Scroll to :menuselection:`Channels --> Email Alias`. In the :guilabel:`Alias`
field, type the desired name for the team's email alias.

.. image:: receiving_tickets/receiving-tickets-email-alias.png
   :align: center
   :alt: View of the settings page of a Helpdesk team emphasizing the email alias feature in Odoo
         Helpdesk.

.. note::
   Custom email domains are **not** required in order to use an email alias, however, they can be
   configured through *Settings* app. If the database does not have a custom domain already
   configured, click :guilabel:`Configure a custom domain` to be redirected to the
   :guilabel:`Settings` page. From there, enable :guilabel:`Custom Email Servers`.

When an email is received, the subject line becomes the title of a new *Helpdesk* ticket. The body
of the email is also added to the ticket under the :guilabel:`Description` tab and in the ticket's
:guilabel:`Chatter`.

.. _receiving_tickets/live-chat:

Live Chat
---------

The *Live Chat* feature lets website visitors connect directly with a support agent or chatbot.
*Helpdesk* tickets can be instantly created during these conversations using the :doc:`response
command </applications/websites/livechat/responses>` `/ticket`.

To enable *Live Chat*, navigate to the :menuselection:`Configuration --> Helpdesk Teams` list view,
select a team, and on the :guilabel:`Teams` settings page, click the checkbox next to
:guilabel:`Live Chat` under the :guilabel:`Channels` heading.

.. note::
   If this is the first time :doc:`Live Chat </applications/websites/livechat>` has been enabled on
   the database, the page may need to be saved manually and refreshed before any further steps can
   be taken.

After the :guilabel:`Live Chat` setting is enabled on a *Helpdesk* team, a new *Live Chat* channel
is created. Click on :guilabel:`Configure Live Chat Channel` to update the channel's settings.

Customize the live chat channel
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

On the channel's settings page, :guilabel:`Channel Name` can be edited, though, Odoo names the
channel to match the *Helpdesk* team name, by default.

.. example::
   If a *Helpdesk* team is named `Customer Care`, a *Live Chat* channel is created called `Customer
   Care`.

   .. image:: receiving_tickets/receiving-tickets-live-chat-new-channel.png
      :align: center
      :alt: View of the Kanban cards for the available Live Chat channels.

On the channel form, navigate through the tabs to complete the setup.

Add operators
*************

*Operators* are the users who act as agents and respond to live chat requests from customers. The
user who created the live chat channel is added by default.

To add additional users, click on the :guilabel:`Operators` tab, click :guilabel:`Add`.


Click the checkbox next to the users to be added, and click :guilabel:`Select`. Click
:guilabel:`New` to create new operators. Then, click :guilabel:`Save & Close`, or :guilabel:`SAVE &
NEW` to add multiple new operators.

.. danger::
   Creating a new user can impact the status of an Odoo subscription, as the total number of users
   in a database counts towards the billing rate. Proceed with caution before creating a new user.
   If a user already exists, adding them as an operator will **not** alter the subscription or
   billing rate for a database.

As well, current operators can be edited or removed by clicking on their respective boxes in the
:guilabel:`Operators` tab, and then adjusting their form values, or by using one of the form buttons
located at the bottom of the form, such as :guilabel:`Remove`.

.. tip::
   Users can add themselves as an operator by clicking the :guilabel:`Join Channel` button on a
   *Live Chat* channel.

   .. image:: receiving_tickets/receiving-tickets-join-live-chat.png
      :align: center
      :alt: View of a live chat channel Kanban card with the join button emphasized.

Modify channel options
**********************

The :guilabel:`Options` tab contains the visual and text settings for the live chat window.

- :guilabel:`Notification Text`: this field updates the greeting displayed in the text bubble when
  the live chat button appears on the website.

- :guilabel:`Welcome Message`: this field changes the first message a visitor receives when they
  open the chat window. This message appears as though it is sent by a live chat operator, and
  should be an invitation to continue the conversation.

- :guilabel:`Chat Input Placeholder`: this field changes the text that appears in the box where
  visitors type their replies. For example, `Ask your question here`.

- :guilabel:`Livechat Button Color` and the :guilabel:`Channel Header Color`: these fields alter the
  color of the live chat button as it appears on the website, and the channel window once a visitor
  opens it to begin a conversation. To change the either of the colors, click a color bubble to open
  the color selection window, then click and drag the circle along the color gradient. Click out of
  the selection window once complete. Click the refresh icon to the right of the color bubbles to
  reset the colors to the default selection.

.. tip::
   Color selection, for the button or header, can be made manually, or through RGB, HSL or HEX code
   selection. Different options are available, depending on the operating system or browser.

Create channel rules
********************

The :guilabel:`Channel Rules` tab determines when the live chat window opens on the website by logic
of when a :guilabel:`URL Regex` action is triggered (e.g., a page visit).

.. tip::
   A regex, or regular expression, is sometimes referred to as a rational expression. It is a
   sequence of characters that specifies a match pattern in text. A match is made within the given
   range of numbers or for the set of characters.

Edit existing rules, or create a new one by clicking :guilabel:`Add a line`, and fill out the pop-up
form details based on how the rule should apply.

To include a :guilabel:`Chatbot` on this channel, select it from the drop-down menu. If the chatbot
should only be active when no operators are available, check the box labeled :guilabel:`Enabled only
if no operator`.

.. note::
   If a :doc:`chatbot </applications/websites/livechat/chatbots>` is added to a live chat channel, a
   new :guilabel:`Chatbots` smart button appears on the channel settings form. Click here to create
   and update the chatbot *script*. Each line in the script contains a :guilabel:`Message`,
   :guilabel:`Step Type`, :guilabel:`Answers`, and conditional *Only If* logic that applies when
   certain pre-filled answers are chosen. To create more steps in the script, click :guilabel:`Add a
   line` and fill out the script steps form according to the desired logic.

Add the URLs for the pages where the channel should appear to in the :guilabel:`URL Regex` field.
Only the path fromthe root domain is needed, not the full URL. If this channel should only be
available to users in specific countries, add them to the :guilabel:`Country` field. If this field
is left blank, the channel will be available to all site visitors.

.. image:: receiving_tickets/receiving-tickets-channel-rules.png
   :align: center
   :alt: View of the Kanban cards for the available Live Chat channels.

Use the live chat widget
************************

The :guilabel:`Widget` tab on the live chat channel form offers a website widget that can be added
to third party websites. Additionally, a URL is available, that can provide instant access to a live
chat window.

The live chat :guilabel:`Widget` can be applied to websites created through Odoo by navigating to
the :menuselection:`Website app --> Configuration --> Settings --> Email & Marketing`. Then scroll
to the :guilabel:`Live Chat` section, and select the channel to add to the site. Click
:guilabel:`Save` to apply.

To add the widget to a website created on a third-party website, click the :guilabel:`Copy` button
next to the first listed code, and paste the code into the `<head>` tag on the site.

To send a live chat session to a customer or supplier, click the :guilabel:`Copy` button next to the
second listed code, and send the URL via email.

Create a support ticket from a live chat session
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Operators who have joined a live chat channel are able to communicate with site visitors in real
time.

During the conversation, an operator can use the shortcut :doc:`command
</applications/websites/livechat/responses>` `/ticket` to create a ticket without leaving the chat
window. The transcript from the conversation is added to the new ticket, under the
:guilabel:`Description` tab.

.. tip::
   *Helpdesk* tickets can also be created through the :doc:`Whatsapp
   </applications/productivity/whatsapp>` app using the same `/ticket` command.

.. _receiving_tickets/website-form:

Website Form
------------

Enabling the *Website Form* setting adds a new page to the website with a customizable form. A new
ticket is created once the required form fields are filled out and submitted.

To activate the website form, navigate to a team's settings page under :menuselection:`Configuration
--> Helpdesk Teams`. Find the :guilabel:`Website Form` feature under the :guilabel:`Help Center`
section, and check the box. If more than one website is active on the database, confirm the correct
website is listed in the :guilabel:`Website` field. If not, select the correct one from the
drop-down list.

After the feature is activated, click the :guilabel:`Go to Website` smart button at the top of the
:guilabel:`Teams` settings page to view and edit the new website form, which is created
automatically by Odoo.

.. note::
   After enabling the website form, the *Teams* settings page may need to be refreshed before the
   *Go to Website* smart button appears.

   As well, if a *Help Center* is published, the smart button navigates there first. Simply click
   the :guilabel:`Contact Us` button at the bottom of the forum to navigate to the ticket
   submission form.

.. image:: receiving_tickets/receiving-tickets-go-to-website.png
   :align: center
   :alt: View of the settings page of a helpdesk team emphasizing the Go to Website button in
         Odoo Helpdesk.

Customize the website ticket form
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

To customize the default ticket submission form, click the :guilabel:`Edit` button in the upper
right corner of the page. This opens the editing pane on the right side of the window. Click on one
of the fields in the form to edit.

To add a new field, go to the :guilabel:`Field` section and click :guilabel:`+Field`. Click the
:guilabel:`🗑️ (trash can)` icon to delete the field. Edit the other options for the new field as
necessary:

- :guilabel:`Type`: which matches an Odoo model value to the field (e.g. `Customer Name`).
- :guilabel:`Input Type`: to determine what type of input the field should be, like `Text`, `Email`,
  `Telephone` or `URL`.
- :guilabel:`Label`: to give the form field a label (e.g. `Full Name`, `Email Address`, etc.). Also
  control the label position on the form by using the nested :guilabel:`Position` options.
- :guilabel:`Description`: which, optionally, adds an editable line under the input box to provide
  additional contextual information related to the field.
- :guilabel:`Placeholder`: to add a sample input value.
- :guilabel:`Default value`: to add common use case values that most customers would find valuable.
  For example, this can include prompts of information customers should include to make it easier to
  solve their issue, such as an account number, or product number.
- :guilabel:`Required`: to mark a field as required in order for the form to be submitted, toggle
  the switch from gray to blue.
- :guilabel:`Visibility`: to allow for absolute or conditional visibility of the field. Nested
  options, such as device visibility, appear when certain options are selected.
- :guilabel:`Animation`: choose whether or not the field should include animation.

.. image:: receiving_tickets/receiving-tickets-web-form.png
   :align: center
   :alt: View of the unpublished website form to submit a ticket for Odoo Helpdesk.

Once the form has been optimized and is ready for public use, :guilabel:`Save` the changes, and then
publish the form by clicking on the :guilabel:`Unpublished` button at the top of the page.

Prioritizing tickets
====================

All tickets include a :guilabel:`Priority` field. The highest priority tickets appear at the top of
the Kanban and list views.

.. image:: receiving_tickets/receiving-tickets-priority.png
   :align: center
   :alt: View of a team's Kanban view and the prioritized tasks in Odoo Helpdesk.

The priority levels are represented by stars:

   - 0 stars = *Low Priority*
   - 1 star = *Medium Priority*
   - 2 stars = *High Priority*
   - 3 stars = *Urgent*

Tickets are set to low priority (0 stars) by default. To change the priority level, select the
appropriate number of stars on the Kanban card, or on the ticket.

.. warning::
   As priority levels can be used as criteria for assigning :doc:`SLAs <sla>`, changing the priority
   level of a ticket can alter the :abbr:`SLA (Service Level Agreement)` deadline.

.. seealso::
   - :doc:`/applications/services/helpdesk/advanced/close_tickets`
   - :doc:`/applications/general/email_communication/email_servers`
   - :doc:`/applications/websites/livechat`
