==========================
Email marketing essentials
==========================

The Odoo *Email Marketing* app provides email design tools, templates, and features to create
engaging emails, and build successful campaigns. The *Email Marketing* app also provides detailed
reporting metrics to track their overall effectiveness.

Email marketing dashboard
=========================

After installing the application, click the :menuselection:`Email Marketing` app icon from the main
Odoo dashboard. Doing so reveals the main :guilabel:`Mailings` dashboard in the default list view.

.. image:: email_marketing_essentials/mailings-dashboard.png
   :align: center
   :alt: View of the main dashboard of the Odoo Email Marketing application.

In the search bar, the default filter of :guilabel:`My Mailings` is present to show all the mailings
related to the current user. To remove that filter, click the :guilabel:`✖️ (remove)` icon next to
the filter in the search bar. Doing so reveals all the mailings in the database.

The information on the :guilabel:`Mailings` dashboard has four different view options, located in
the upper-right corner as individual icons.

The view options, from left-to-right, are:

- :ref:`List <email_marketing/email_marketing_templates/list>` (default view)
- :ref:`Kanban <email_marketing/email_marketing_templates/kanban>`
- :ref:`Calendar <email_marketing/email_marketing_templates/calendar>`
- :ref:`Graph <email_marketing/email_marketing_templates/graph>`

.. _email_marketing/email_marketing_templates/list:

List view
---------

The list view, represented by the :guilabel:`☰ (horizontal lines)` icon in the upper-right corner,
is the default view of the :guilabel:`Mailings` dashboard in the *Email Marketing* app.

While in list view, there are columns dedicated to different aspects of information related to the
listed emails. Those columns are as follows:

- :guilabel:`Date`: the date the email was sent.
- :guilabel:`Subject`: the subject of the email.
- :guilabel:`Responsible`: the user who created the email.
- :guilabel:`Sent`: how many times the email has been sent.
- :guilabel:`Delivered (%)`: percentage of sent emails that have been successfully delivered.
- :guilabel:`Opened (%)`: percentage of sent emails that have been opened by the recipients.
- :guilabel:`Clicked (%)`: percentage of sent emails that have been clicked by the recipients.
- :guilabel:`Replied (%)`: percentage of sent emails that have been replied to by the recipients.
- :guilabel:`Status`: the status of the email (:guilabel:`Draft`, :guilabel:`In Queue`, or
  :guilabel:`Sent`).

To add or remove columns, click the :guilabel:`Additional Options (two horizontal lines with dots)`
icon, located to the far-right of the column titles in list view. Doing so reveals a drop-down menu
of additional column options.

.. _email_marketing/email_marketing_templates/kanban:

Kanban view
-----------

The kanban view, represented by the :guilabel:`inverted bar graph` icon, can be accessed in the
upper-right corner of the :guilabel:`Mailings` dashboard in the *Email Marketing* application.

.. image:: email_marketing_essentials/kanban-view.png
   :align: center
   :alt: Kanban view of the main dashboard of the Odoo Email Marketing application.

While in kanban view, the email information is displayed in the various stages.

The stages are: :guilabel:`Draft`, :guilabel:`In Queue`, :guilabel:`Sending`, :guilabel:`Sent`.

- :guilabel:`Draft`: the email is still being written/created.
- :guilabel:`In Queue`: the email is scheduled, and sent at a later date.
- :guilabel:`Sending`: the email is currently being sent to its recipients.
- :guilabel:`Sent`: the email has already been sent to its recipients.

In each stage, there are drag-and-drop cards representing the emails that have been created/sent,
and the stage they are in represents the current status of that mailing.

Each mailing block on the :guilabel:`Mailings` dashboard provides key information related to that
specific email.

When the cursor hovers over the upper-right corner of an email campaign card, :guilabel:`⋮ (three
vertical dots)`) appear. When clicked, a mini drop-down menu reveals the option to color-code the
email, :guilabel:`Delete` the email, or :guilabel:`Archive` the message for potential future use.

.. image:: email_marketing_essentials/three-dot-dropdown.png
   :align: center
   :alt: View of the three-dot drop-down menu on the Odoo Email Marketing dashboard.

.. _email_marketing/email_marketing_templates/calendar:

Calendar view
-------------

The calendar view, represented by a :guilabel:`📆 (calendar)` icon, can be accessed in the
upper-right corner of the :guilabel:`Mailings` dashboard in the *Email Marketing* app.

While in calendar view, a monthly calendar (by default), shows when the mailings have been sent or
are scheduled to be sent.

.. image:: email_marketing_essentials/calendar-view.png
   :align: center
   :alt: Calendar view of the mailings dashboard in the Email Marketing application.

The current date is represented by a :guilabel:`🔴 (red circle)` icon over the date on the calendar.

To the right of the calendar, the options to filter the results by :guilabel:`Responsible` and/or
:guilabel:`Status` are available, via checkboxes.

.. tip::
   To hide this sidebar, click the :guilabel:`white and black box` icon, located above the sidebar.

In the top-left corner, above the calendar, the option to change the time period being displayed is
available via a drop-down menu, which shows :guilabel:`Month`, by default. When clicked, the
drop-down menu that appears reveals the options: :guilabel:`Day`, :guilabel:`Week`,
:guilabel:`Month` (default), :guilabel:`Year`, and :guilabel:`Show weekends` (selected by default).

Clicking any of those options changes the calendar display to reflect that desired amount of time.

Clicking either :guilabel:`⬅️ (left arrow)` icon or :guilabel:`➡️ (right arrow)` icon changes the
calendar to a previous or future time, depending on what's clicked, based on the chosen amount of
time being represented.

To jump back to the current date, click the :guilabel:`Today` button.

.. _email_marketing/email_marketing_templates/graph:

Graph view
----------

The graph view, represented by a :guilabel:`line graph` icon, can be accessed in the upper-right
corner of the :guilabel:`Mailings` dashboard in the *Email Marketing* app.

While in graph view, the status of the emails on the :guilabel:`Mailings` page is represented in a
bar graph, but other graph view options can be implemented, if needed.

.. image:: email_marketing_essentials/graph-view.png
   :align: center
   :alt: How the Graph view appears in the Odoo Email Marketing application.

In the upper-left corner, above the graph, there is a :guilabel:`Measures` drop-down menu. When
clicked, different filter options become available to further customize the graph views.

Those :guilabel:`Measures` options are: :guilabel:`A/B Testing percentage` and :guilabel:`Count`
(default).

To the right of the :guilabel:`Measures` drop-down menu is an :guilabel:`Insert in Spreadsheet`
button. When clicked, a pop-up window appears, in which the ability to add the graph to a
spreadsheet or dashboard becomes available.

Beside the :guilabel:`Measures` drop-down menu and :guilabel:`Insert in Spreadsheet` button are
different graph view options. From left-to-right, those graph view options are: :guilabel:`bar
chart` (default), :guilabel:`line chart`, and :guilabel:`pie chart`.

.. note::
   Each graph view option provides its own series of additional view options, which appear to the
   right of the selected graph view option.

Search options
--------------

Regardless of the view chosen for the :guilabel:`Mailings` dashboard in the *Email Marketing* app,
the :guilabel:`Filters`, :guilabel:`Group by`, and :guilabel:`Favorites` options are always
available to furhter customize the information being displayed.

To access those options, click the :guilabel:`downward arrow` icon, located to the right of the
search bar. Doing so reveals a drop-down mega menu featuring those filtering and grouping options.

.. image:: email_marketing_essentials/search-mega-menu.png
   :align: center
   :alt: The drop-down mega menu of search options the Odoo Email Marketing application.

These options provide various ways to specify and organize the information seen on the
:guilabel:`Mailings` dashboard in the *Email Marketing* application.

.. tabs::

   .. tab:: Filters

      This section of the drop-down mega menu provides different ways to filter email results being
      shown on the :guilabel:`Mailings` dashboard in the *Email Marketing* app.

      .. image:: email_marketing_essentials/filters-dropdown.png
         :align: center
         :alt: View of filters drop-down menu options on the Odoo Email Marketing dashboard.

      The options are: :guilabel:`My Mailings`, :guilabel:`Sent Date`, :guilabel:`A/B Tests`,
      :guilabel:`A/B Tests to review`, :guilabel:`Archived`, and :guilabel:`Add Custom Filter`.

      If :guilabel:`Add Custom Filter` is selected, Odoo reveals a pop-up window, with three
      customizable fields to fill in, in order to create custom filter rules for Odoo to use to
      retrieve results that fit more specific criteria.

      .. image:: email_marketing_essentials/add-custom-filter-popup.png
         :align: center
         :alt: Add custom filter pop-up window that appears in Odoo Email Marketing app.

   .. tab:: Group By

      This section of the drop-down mega menu provides different ways to group email results being
      shown on the :guilabel:`Mailings` dashboard in the *Email Marketing* app.

      .. image:: email_marketing_essentials/group-by-dropdown.png
         :align: center
         :alt: View of the Group By drop-down menu on the Odoo Email Marketing application.

      Using this section, the data can be grouped by the messages' :guilabel:`Status`, or who it was
      :guilabel:`Sent By`.

      There is also the option to group the data by :guilabel:`Sent Period`, which has its own
      sub-menu of options to choose from. The :guilabel:`Sent Period` options are :guilabel:`Year`,
      :guilabel:`Quarter`, :guilabel:`Month`, :guilabel:`Week`, and :guilabel:`Day`.

      If none of the above :guilabel:`Group By` options deliver the desired results, click
      :guilabel:`Add Custom Group` at the bottom of the :guilabel:`Group By` section. Doing so
      reveals a drop-down menu, wherein custom criteria can be selected and applied, thus delivering
      any grouping of data that may be desired.

   .. tab:: Favorites

      This section provides the opportunity to save custom filters and/or groupings for future use.
      To utilize this section, click the :guilabel:`Save current search` field, which reveals
      additional fields.

      .. image:: email_marketing_essentials/favorites-dropdown.png
         :align: center
         :alt: View of the Favorites drop-down menu on the Odoo Email Marketing application.

      Give the favorited filter/grouping a title on the blank line above the checkboxes for
      :guilabel:`Default filter` and :guilabel:`Shared`.

      Ticking the box for :guilabel:`Default filter` makes this favorited filter/grouping the
      default option. Ticking the box for :guilabel:`Shared` allows other users to see and use this
      favorited filter/grouping.

      When all desired options are configured, click :guilabel:`Save` to save the filter/grouping in
      the :guilabel:`Favorites` section of the mega drop-down menu.

Settings
========

To view (and modify) the *Email Marketing* settings, navigate to :menuselection:`Email Marketing
application --> Configuration --> Settings`.

.. image:: email_marketing_essentials/configuration-settings.png
   :align: center
   :alt: View of the Configuration menu with Settings page in the Odoo Email Marketing application.

On the :guilabel:`Settings` page, there are four features available.

.. image:: email_marketing_essentials/settings.png
   :align: center
   :alt: View of the Settings page in the Odoo Email Marketing application.

The features are:

- :guilabel:`Mailing Campaigns`: enables the option to manage mass mailing campaigns.
- :guilabel:`Blacklist Option when Unsubscribing`: allows recipients to blacklist themselves from
  future mailings during the unsubscribing process.
- :guilabel:`Dedicated Server`: provides the option to utilize a separate, dedicated server for
  mailings. When enabled, Odoo reveals a new field (and link), in which the specific server
  configurations must be entered, in order for it to connect properly to Odoo.
- :guilabel:`24H Stat Mailing Reports`: allows users to check how well mailings have performed a day
  after it has been sent.

Create an email
===============

To create an email, open the :menuselection:`Email Marketing` application, and click the
:guilabel:`New` button in the upper-left corner of the :guilabel:`Mailings` dashboard page.

Clicking :guilabel:`New` reveals a blank email form.

.. image:: email_marketing_essentials/blank-email-detail-form.png
   :align: center
   :alt: View of a blank email detail form in Odoo Email Marketing application.

On the email form, there are fields for the :ref:`Subject
<email_marketing/email_marketing_templates/subject>` and :ref:`Recipients
<email_marketing/email_marketing_templates/recipients>` of the email.

Beneath that, there are three tabs: :ref:`Mail Body
<email_marketing/email_marketing_templates/mail_body>`, :ref:`A/B Tests
<email_marketing/email_marketing_templates/ab_tests>`, and :ref:`Settings
<email_marketing/email_marketing_templates/settings_tab>`.

.. _email_marketing/email_marketing_templates/subject:

Subject
-------

First, enter a :guilabel:`Subject` to the email. The :guilabel:`Subject` is visible in the
recipients' inbox, allowing them to get quickly see what the message is about.

.. note::
   The :guilabel:`Subject` field is mandatory. An email can **not** be sent without a
   :guilabel:`Subject`.

The :guilabel:`smiley face with a plus sign` icon at the end of the :guilabel:`Subject` field
represents emojis that can be added to the :guilabel:`Subject` field. Clicking that icon reveals a
pop-up menu of emojis that can be used.

Beside the :guilabel:`smiley face with a plus sign` icon at the end of the :guilabel:`Subject` field
is an empty :guilabel:`star` icon. When clicked, the :guilabel:`star` icon turns gold, and the email
is saved as a template in the :guilabel:`Mail Body` tab, which can be used again in the future.

.. _email_marketing/email_marketing_templates/recipients:

Recipients
----------

Beneath the :guilabel:`Subject` field on the email form is the :guilabel:`Recipients` field. In this
field select the recipients of the email. By default, the :guilabel:`Mailing List` option is
selected, but clicking the field reveals a drop-down menu of other recipient options.

With the default :guilabel:`Mailing List` option selected, a specific :guilabel:`Mailing List`
**must** be chosen from the adjacent :guilabel:`Select mailing lists` field drop-down menu.

.. tip::
   More than one mailing list can be chosen from the :guilabel:`Select mailing lists` field.

Odoo then sends the email to contacts on that specific mailing list(s).

.. seealso::
   :doc:`/applications/marketing/email_marketing/mailing_lists`

When the :guilabel:`Recipients` field is clicked, a drop-down menu of other options is revealed.
Each option provides different ways Odoo can create a target audience for the email.

.. image:: email_marketing_essentials/recipients-dropdown.png
   :align: center
   :alt: View of recipients drop-down menu in the Odoo Email Marketing application.

Those options (excluding the default :guilabel:`Mailing List`) provide the option to create a more
specified recipient filter, in an equation-like format, which appears beneath the
:guilabel:`Recipients` field.

The :guilabel:`Recipients` field options, other than the default :guilabel:`Mailing List` option,
are as follows:

- :guilabel:`Contact`: focuses on specific contacts in the database.
- :guilabel:`Event Registration`: focuses on people in the database who purchased event
  registrations.
- :guilabel:`Lead/Opportunity`: focuses on leads or opportunities in the database.
- :guilabel:`Mailing Contact`: focuses on specific mailing contacts in the database.
- :guilabel:`Sales Order`: focuses on a specific sales orders in the database.

Add recipient filter
~~~~~~~~~~~~~~~~~~~~

To add a more specified recipient filter to any :guilabel:`Recipient` option, select any recipient
option (other than :guilabel:`Mailing List`), and click the :guilabel:`Modify filter (right-facing
arrow)` icon beneath the :guilabel:`Recipient` field, if needed, to reveal three subsequent filter
rule fields, formatted like an equation.

To reveal the sub-menu options within the filter rule fields, click each field, and make the desired
selections, until the preferred configuration has been achieved.

The number of :guilabel:`Records` in the database that match the configured rule(s) are indicated
beneath the configured filter rule(s), in green.

.. image:: email_marketing_essentials/filter-records.png
   :align: center
   :alt: View of how recipient filters can be customized in Odoo Email Marketing.

.. note::
   Some sub-menu options in the first rule field allow for a second choice to provide even more
   specificity.

To the right of each rule, are :guilabel:`➕ (Add node)`, and :guilabel:`(Add branch)`, :guilabel:`🗑️
(Delete node)`, icons.

The :guilabel:`➕ (Add node)` icon adds a node (line) to the rule.

The :guilabel:`(Add branch)` icon adds a branch to the node. A branch means two additional, indented
sub-nodes are added to the rule, providing even more specificity to the line above it.

The :guilabel:`🗑️ (Delete node)` icon deletes a specific node (line) of the rule.

.. _email_marketing/email_marketing_templates/mail_body:

Mail body tab
-------------

In the :guilabel:`Mail Body` tab, there are a number of pre-configured message templates to choose
from.

.. image:: email_marketing_essentials/mail-body-templates.png
   :align: center
   :alt: View of the templates in the Mail Body tab in Odoo Email Marketing application.

Select the desired template, and proceed to modify every element of its design details with Odoo's
drag-and-drop building blocks, which appear on the right sidebar when a template is chosen.

.. image:: email_marketing_essentials/template-building-blocks.png
   :align: center
   :alt: View of the building blocks in the Mail Body tab in Odoo Email Marketing application.

The features on the sidebar used to create and customize emails are separated into three sections:
:guilabel:`Blocks`, :guilabel:`Customize`, and :guilabel:`Design`.

Each building block provides unique features and professional design elements. To use a building
block, drag-and-drop the desired block element onto the body of the email being built. Once dropped,
various aspects of the building block can be customized.

.. tip::
   To build an email from the ground up, without any building block elements, select the
   :guilabel:`Plain Text` template. When selected, Odoo provides a completely blank email canvas,
   which can be customized in a number of way using the front-end rich text editor that accepts
   slash `/` commands.

   When `/` is typed into the blank body of the email, while using a :guilabel:`Plain Text`
   template, a drop-down menu of various design options and elements appears, which can be used to
   create the desired email design.

   .. image:: email_marketing_essentials/template-blank-slash.png
     :align: center
     :alt: View of the rich text editor drop-down in the Odoo Email Marketing application.

.. _email_marketing/email_marketing_templates/ab_tests:

A/B tests tab
-------------

Initially, when the :guilabel:`A/B Tests` tab is opened on an email form, the only option available
is :guilabel:`Allow A/B Testing`. This is **not** a required option.

If this option is enabled, recipients are only mailed *once* for the entirety of the campaign.

This allows the user to send different versions of the same mailing to randomly selected recipients
to gauge the effectiveness of various designs, formats, layouts, content, and so on -- without any
duplicate messages being sent.

When the checkbox beside :guilabel:`Allow A/B Testing` is ticked, an :guilabel:`on (%)` field
appears, in which the user determines the percentage of the pre-configured recipients are going to
be sent this current version of the mailing as part of the test.

.. note::
   The default figure in the :guilabel:`on (%)` field is `10`, but that figure can be changed at any
   time.

Beneath that, two additional fields appear:

The :guilabel:`Winner Selection` field provides a drop-down menu of options, wherein the user
decides what criteria results should be used to determine the "winning" version of the email tests
that are sent.

The options in the :guilabel:`Winner Selection` field are as follows:

- :guilabel:`Manual`: allows the user to detemine the "winning" version of the mailing. This option
  removes the :guilabel:`Send Final On` field.
- :guilabel:`Highest Open Rate` (default): the mailing with the highest open rate is determined to
  be the "winning" version.
- :guilabel:`Highest Click Rate`: the mailing with the highest click rate is determined to be the
  "winning" version.
- :guilabel:`Highest Reply Rate`: the mailing with the highest reply rate is determined to be the
  "winning" version.
- :guilabel:`Leads`: the mailing with the most leads generated is determined to be the "winning"
  version.
- :guilabel:`Quotations`: the mailing with the most quotations generated is determined to be the
  "winning" version.
- :guilabel:`Revenues`: the mailing with the most revenue generated is determined to be the
  "winning" version.

The :guilabel:`Send Final On` field allows users to choose a date that is used to know *when* Odoo
should determine the "winning" email, and subsequently, send that version of the email to the
remaining recipients.

.. image:: email_marketing_essentials/ab-test-tab.png
   :align: center
   :alt: View of the A/B Tests tab in Odoo Email Marketing application.

To the right of those fields is a :guilabel:`Create an Alternate Version` button. When clicked, Odoo
presents a new :guilabel:`Mail Body` tab for the user to create an alternate version of the email to
test.

.. _email_marketing/email_marketing_templates/settings_tab:

Settings tab
------------

The options present in the :guilabel:`Settings` tab of the mail form are divided into two sections:
:guilabel:`Email Content` and :guilabel:`Tracking`.

.. note::
   The options available in the :guilabel:`Settings` tab are different, depending on if the
   :guilabel:`Mailing Campaigns` feature is activated in the :guilabel:`Settings` page of the *Email
   Marketing* application (:menuselection:`Email Marketing --> Configuration --> Settings`).

Without the :guilabel:`Mailing Campaigns` feature activated, the :guilabel:`Settings` tab on the
email form looks like this:

.. image:: email_marketing_essentials/settings-without-features.png
   :align: center
   :alt: View of settings tab in Odoo Email Marketing app, without campain setting activated.

Email content
~~~~~~~~~~~~~

- :guilabel:`Preview Text`: allows user to enter a preview sentence to encourage recipients to open
  the email. In most inboxes, this is dsiplayed next to the subject. If left empty, the first
  characters of the email content appear, instead. The ability to add an emoji in this field is
  available, as well, via the :guilabel:`smiley face with a plus sign` icon.
- :guilabel:`Send From`: designate an email alias that displays as the sender of this particular
  email.
- :guilabel:`Reply To`: designate an email alias to whom all the replies of this particular email
  are sent.
- :guilabel:`Attach a file`: if any specific files are required (or helpful) for this email, click
  the :guilabel:`Attachments` button, and proceed to upload and attach the desired file(s) to the
  email.

Tracking
~~~~~~~~

- :guilabel:`Responsible`: designate a user in the database to be responsible for this particular
  email.

.. note::
   If the :guilabel:`Mailing Campaign` feature *is* activated, an additional :guilabel:`Campaign`
   field appears in the :guilabel:`Tracking` section of the :guilabel:`Settings` tab.

      .. image:: email_marketing_essentials/settings-tab-with-campaign.png
         :align: center
         :alt: View of settings tab in Odoo Email Marketing when campaign setting is activated.

   The additional :guilabel:`Campaign` field allows users to attach this particular email to a
   mailing campaign, if desired.

   If the desired campaign isn't available in the initial drop-down menu, select :guilabel:`Search
   More` to reveal a complete list of all mailing campaigns in the database.

   Or, type the name of the desired mailing campaign in the :guilabel:`Mailing Campaign` field,
   until Odoo reveals the desired campaign in the drop-down menu. Then, select the desired campaign.

Send, schedule, test
====================

Once the mailing is finalized, the following options can be utilized, via buttons located in the
upper-left corner of the email form: :ref:`Send <email_marketing/email_marketing_templates/send>`,
:ref:`Schedule <email_marketing/email_marketing_templates/schedule>`, and :ref:`Test
<email_marketing/email_marketing_templates/test>`.

.. _email_marketing/email_marketing_templates/send:

Send
----

The :guilabel:`Send` button reveals a :guilabel:`Ready to unleash emails?` pop-up window.

.. image:: email_marketing_essentials/send-popup.png
   :align: center
   :alt: View of pop-up window that appears when the send button on an email form is clicked.

When the :guilabel:`Send to all` button is clicked, Odoo sends the email to the desired recipients.
Once, Odoo has sent the mailing, the status changes to :guilabel:`Sent`.

.. _email_marketing/email_marketing_templates/schedule:

Schedule
--------

The :guilabel:`Schedule` button reveals a :guilabel:`When do you want to send your mailing?` pop-up
window.

.. image:: email_marketing_essentials/schedule-popup.png
   :align: center
   :alt: View of pop-up window that appears when the schedule button on an email form is clicked.

In this pop-up window, click the :guilabel:`Send on` field to reveal a calendar pop-up window.

.. image:: email_marketing_essentials/schedule-popup-calendar.png
   :align: center
   :alt: View of pop-up window that appears when the schedule button on an email form is clicked.

From the calendar pop-up window, select the future date-time for Odoo to send this email. Then,
click :guilabel:`✔️ (checkmark) Apply`. When a date-time is chosen, click the :guilabel:`Schedule`
button, and the status of the mailing changes to :guilabel:`In Queue`.

.. _email_marketing/email_marketing_templates/test:

Test
----

The :guilabel:`Test` button reveals a :guilabel:`Test Mailing` pop-up window.

.. image:: email_marketing_essentials/test-popup.png
   :align: center
   :alt: View of pop-up window that appears when the test button on an email form is clicked.

From this pop-up window, enter the email addresses of the contacts to whom Odoo should send this
test email in the :guilabel:`Recipients` field. Multiple contacts can be added in this field, if
desired.

Once all the desired email addresses have been entered in the :guilabel:`Recipients` field, click
the :guilabel:`Send Test` button.

.. warning::
   By default, there's a daily limit applied for **all emails** sent throughout *all* applications.
   So, if there are remaining emails to be sent after a limit has been reached, those mailings *are
   not* sent automatically the next day. The sending needs to be forced, by opening the email and
   clicking :guilabel:`Retry`.

Mailing campaigns
=================

The *Email Marketing* application provides users with the ability to build mailing campaigns.

In order to create and customize mailing campaigns, the :guilabel:`Mailing Campaigns` **must** be
activated in the :guilabel:`Settings` page of the *Email Marketing* application. To do that,
navigate to :menuselection:`Email Marketing app --> Configuration --> Settings`, tick the box beside
:guilabel:`Mailing Campaigns`, and click the :guilabel:`Save` button.

.. image:: email_marketing_essentials/campaigns-feature.png
   :align: center
   :alt: View of the campaign feature setting in Odoo Email Marketing.

Once the :guilabel:`Mailing Campaigns` feature is activated, a new :guilabel:`Campaigns` menu option
appears in the header.

When that is clicked, Odoo reveals a separate :guilabel:`Campaigns` page, displaying all the mailing
campaigns in the database, and the current stage they are in, showcased in a default kanban view.

.. image:: email_marketing_essentials/campaigns-page.png
   :align: center
   :alt: View of the campaign page in Odoo Email Marketing.

.. note::
   This information can also be viewed in a list, by clicking the :guilabel:`☰ (horizontal lines)`
   icon in the upper-right corner.

Clicking any campaign from the :guilabel:`Campaigns` page reveals that campaign's form.

There are two different ways to create and customize campaigns in the *Email Marketing* application,
either directly from the :ref:`Campaigns page
<email_marketing/email_marketing_templates/campaign-page>` or through the :ref:`Settings tab
<email_marketing/email_marketing_templates/campaign-settings>` on an email form.

.. _email_marketing/email_marketing_templates/campaign-page:

Create mailing campaign (from campaigns page)
---------------------------------------------

When the :guilabel:`Mailing Campaigns` feature is activated, a new :guilabel:`Campaigns` option
appears in the header of the *Email Marketing* application. Campaigns can be created directly on the
:guilabel:`Campaigns` page in the *Email Marketing* app.

To do that, navigate to :menuselection:`Email Marketing app --> Campaigns --> New`.

Kanban view
~~~~~~~~~~~

When the :guilabel:`New` button is clicked, in the default kanban view on the :guilabel:`Campaigns`
page, a pop-up kanban card appears in the :guilabel:`New` stage.

.. image:: email_marketing_essentials/campaigns-kanban-popup.png
   :align: center
   :alt: View of the campaign pop-up kanban in Odoo Email Marketing.

The same result can be accomplished by clicking the :guilabel:`➕ (plus sign)` at the top of any
kanban stage on the :guilabel:`Campaigns` page.

When the new campaign kanban card appears, the options to enter a :guilabel:`Campaign Name`, add a
:guilabel:`Responsible`, and add :guilabel:`Tags` becomes readily available.

To add the campaign to the kanban stage, click the :guilabel:`Add` button.

To delete the campaign, click the :guilabel:`🗑️ (trash can)` icon.

To futher customize the campaign, click the :guilabel:`Edit` button, which reveals the campaign form
for additional modifications.

.. note::
   A :guilabel:`Campaign Name` **must** be entered in the kanban card, in order for the
   :guilabel:`Edit` button to reveal the campaign form for further modifications.

List view
~~~~~~~~~

To enter the list view on the :guilabel:`Campaigns` page, click the :guilabel:`☰ (horizontal lines)`
icon in the upper-right corner. Doing so reveals all campaign information in a list format.

.. image:: email_marketing_essentials/campaign-page-list-view.png
   :align: center
   :alt: View of the campaign page in list view in Odoo Email Marketing.

To create a campaign form the :guilabel:`Campaigns` page, while in list view, click the
:guilabel:`New` button. Doing so reveals a blank campaign form.

.. image:: email_marketing_essentials/blank-campaign-form.png
   :align: center
   :alt: View of the blank campaign form in Odoo Email Marketing.

From this campaign form, a :guilabel:`Campaign Name` can be entered, a :guilabel:`Responsible` can
be designated, and :guilabel:`Tags` can be added.

At the top of the form, various metric-related smart buttons can be seen that showcase specific
analytics related to the campaign. Those smart buttons are: :guilabel:`Revenues`,
:guilabel:`Quotations`, :guilabel:`Opportunities`, and :guilabel:`Clicks`.

.. note::
   Once a :guilabel:`Campaign Name` is entered, and saved (either manually or automatically),
   additional buttons appear at the top of the form.

   Those additional buttons are: :guilabel:`Send Mailing` and :guilabel:`Send SMS`.

   These button appear automatically when a campaign form is accessed from kanban view because a
   :guilabel:`Campaign Name` **must** be entered in order for the :guilabel:`Edit` button to reveal
   the campaign form.

Campaign form
-------------

On the campaign form (after clicking :guilabel:`Edit` from the kanban card, or selecting an existing
campaign from the :guilabel:`Campaigns` page) there are additional options and metrics available.

.. image:: email_marketing_essentials/campaign-form.png
   :align: center
   :alt: View of the campaign form in Odoo Email Marketing.

At the top of the form, various metric-related smart buttons can be seen that showcase specific
analytics related to the campaign. Those smart buttons are: :guilabel:`Revenues`,
:guilabel:`Quotations`, :guilabel:`Opportunities`, and :guilabel:`Clicks`.

There are also buttons to :guilabel:`Send Mailing`, :guilabel:`Send SMS`, :guilabel:`Add Post`, and
:guilabel:`Add Push` (push notification).

.. note::
   If the :guilabel:`Send Mailing` and :guilabel:`Send SMS` buttons are not readily available, enter
   a :guilabel:`Campaign Name`, then save (either manually or automatically). Doing so reveals those
   buttons.

The status of the campaign can be viewed in the upper-right corner of the campaign form, as well.

.. _email_marketing/email_marketing_templates/campaign-settings:

Create mailing campaign (from settings tab)
-------------------------------------------

To create a new campaign from the :guilabel:`Settings` tab of a mail form, click the
:guilabel:`Campaign` field, and start typing the name of the new campaign. Then, select either
:guilabel:`Create "[Campaign Name]"` or :guilabel:`Create and Edit...` from the drop-down menu that
appears.

.. image:: email_marketing_essentials/mailing-campaign-settings.png
   :align: center
   :alt: View of the mailing campaign creation in the Settings tab of an email form.

Select :guilabel:`Create` to add this new mailing campaign to the database, and modify its settings
in the future.

Select :guilabel:`Create and Edit...` to add this new mailing campaign to the database, and reveal a
:guilabel:`Create Campaign` pop-up window.

.. image:: email_marketing_essentials/mailing-campaign-popup.png
   :align: center
   :alt: View of the email mailing campaign pop-up window in Odoo Email Marketing application.

Here, the new mailing campaign can be further customized. Users can adjust the :guilabel:`Campaign
Name`, assign a :guilabel:`Responsible`, and add :guilabel:`Tags`.

Buttons to :guilabel:`Add Post` or :guilabel:`Send Push` (push notifications) are also available.

There is also a status located in the upper-right corner of the :guilabel:`Create Campaign` pop-up
window, as well.

When all modifications are ready to be finalized, click :guilabel:`Save & Close`. To delete the
entire campaign, click :guilabel:`Discard`.

.. seealso::
   - :doc:`/applications/marketing/email_marketing/mailing_lists`
   - :doc:`/applications/marketing/email_marketing/unsubscriptions`
