**************************************
How To: Use the GDPR Compliance Add-on
**************************************

.. contents::
   :backlinks: none
   :local:

========================================
Step 1. Install and Configure the Add-on
========================================

#. In the Administration panel, go to **Add-ons → Manage add-ons**.

#. Find the **GDPR Compliance (EU)** add-on and click **Install** next to it.

   .. image:: img/gdpr-addon.png
       :align: center
       :alt: The GDPR Compliance add-on first appeared in CS-Cart and Multi-Vendor 4.7.4.

#. Once the add-on is installed, click on its name to open the add-on's settings.

#. On the **Settings → General** tab you'll find the following settings:

   * **Cookie consent**—determines if customers will be notified about cookies, and whether or not they'll have to accept the use of cookies before being allowed to use the site.

     * *None*—customers won't be notified at all that the web-site uses cookies.

     * *Implicit*—customers will see an unobtrusive pop-up notifying them that the web-site uses cookies. Depending on what pages the customers visit, cookies may be set on their devices without their prior approval.

     * *Explicit*—before a customer can enter the web-site, he or she will see the a page with the information that the web-site uses cookies. Customers must give their consent before they can proceed to see the site. That way no cookies are set on customers' devices before the consent is given.

       .. note::

           The ability to ask for explicit consent for the use of cookies first appeared in version 4.8.1. Until then, store owners could only ask for implicit consent under **Settings → Security settings** in the administration panel.

   .. image:: img/gdpr-cookies.png
       :scale: 50%
       :align: center
       :alt: The ability to ask for explicit consent for cookies first appeared in version 4.8.1.

   * **Privacy policy page**—determines at what page from the list on the **Website → Pages** you will have your privacy policy. 

   The add-on's settings also have the **GDPR** tab; there you'll be able to choose where to show the notifications about personal data processing, and edit the texts of those notifications. We'll do it later, in Step 4.

#. Click **Save**.

============================================
Step 2. Add a Cookie Consent Form (Optional)
============================================

Starting from the version 4.15.1, CS-Cart brings a cookie consent form. Visitors see the list of services that set cookies, and what they do. This is necessary for meeting the demands of privacy-related laws like the European Union's GDPR.

To let your customers choose which cookies to accept, set **Cookie consent** to *Explicit* in the **GDPR** add-on settings. After successful setting customers will see a small notification with a request for enabling additional services that require cookies. There visitors customize the services and their respective cookies that you use on your website. All optional cookies (that do not affect the ability to place an order) can be disabled, if a visitor chooses so. A link to the privacy policy placed on this consent will lead to the page you've specified on Step 1.

Let your visitors make a change on their decision, when they want to deactivate or activate services as they see fit. For this, add a link code, for example to your privacy policy page, and customers will be able to choose cookies again. The Klaro service that is used for cookie consent allows to add a link to the website content::

  <a class="button is-success" onclick="return klaro.show();">Change consent settings</a>

.. image:: img/gdpr-change-consent.png
    :align: center
    :alt: Changing cookie consent settings.

.. _gdpr-data-request-buttons:

========================================================
Step 3. Add Buttons for Data-Related Requests (Optional)
========================================================

.. note::

    This step is only possible starting with version 4.8.1. The previous versions don't have the block described in this step.

The GDPR requires you to give customers the data you have about them, or anonymize their personal data on request. By default, customers are supposed to contact you by email regarding this. However, there's a way to make it more convenient for customers: they'd be able to send you a request with a couple of clicks.

#. Go to **Design → Layouts**.

#. Switch to the **Profiles** tab.

#. :doc:`Add a new block </user_guide/look_and_feel/layouts/blocks/actions_on_blocks>`; when doing so, switch to the **Create New Block** tab and choose **GDPR**. That's the block that contains the buttons for contacting store owners.

   .. image:: img/gdpr-block.png
       :align: center
       :alt: Adding a block with GDPR data-related buttons.

#. Once the block has been added, return to the storefront and sign in to an account.

#. Open the profile details page. The new block should now appear where you placed it. It provides 2 buttons:

   * *Send me my data*

   * *Remove my data*

   By clicking these buttons, customers will be able to leave a comment and send a corresponding email to the *User department email address*. If you only have one storefront (or if you use Multi-Vendor), this email address will be taken from **Settings → Company**. If you have multiple storefronts in CS-Cart, then the address will be taken from the settings of the storefront that a customer visits.

   .. important::

       Once the emails are received, it is up to the administrators to :doc:`export personal data or anonymize those customers </user_guide/users/customers/gdpr>`.

   .. image:: img/gdpr-buttons.png
       :align: center
       :alt: The buttons for requesting personal data or its removal as they appear on the storefrnot.

If you intend to use this way, make sure to update the data processing notifications afterwards (we'll be doing it in step 3). The default notifications don't describe this simplified way of contacting you about GDPR-related questions.

============================================
Step 4. Check and Update the Privacy Notices
============================================

The settings of the **GDPR Compliance (EU)** add-on have the **GDPR** tab. It contains the list of places where checkboxes for requesting consent will be displayed. For each place, you can choose whether or not you want a checkbox for requesting consent to appear.

.. image:: img/gdpr-checkboxes.png
    :scale: 30%
    :align: center
    :alt: The notices about personal data processing can be edited separately from each other.

Every checkbox for requesting consent is accompanied by a notice about personal data processing. The texts of these notifications and checkboxes can be accessed and edited separately from each other. These texts are in fact :doc:`language variables </user_guide/look_and_feel/languages/translate>`, so the same rules apply when you translate or edit them.

The texts may have ``[email]`` or ``[company]`` in them. These are placeholders that will be automatically replaced with actual data when customers see the notifications.

If you only have one storefront (or if you use Multi-Vendor), the data for the placeholders will be taken from **Settings → Company**. If you have multiple storefronts in CS-Cart, then the data will be taken from the settings of the storefront that a customer visits:

* ``[company]`` will be taken from *Company name*.

* ``[email]`` will be taken from *User department e-mail address*.

We tried our best to make the default personal data processing notifications as informative as possible. However, we can't guarantee that they fully comply with the GDPR, especially since the practices regarding personal data differ in every company. That's why we ask you to review and edit these notifications as you and your lawyers see fit.

.. hint::

    If you don't want the notification to be too long, add a link to your Privacy Policy to all of them, and describe everything in the Privacy Policy. However, we can't guarantee that this practice is GDPR-compliant, so you'd have to consult your lawyer regarding this.

================================
Step 5. See How the Add-on Works
================================

#. Check the storefront. Make sure that the notifications about personal data processing appear in every place where you collect personal data.

   .. image:: img/gdpr-storefront.png
       :align: center
       :alt: A notification about personal data processing on the storefront.

   For example, the add-on **doesn't** automatically add notifications about personal data processing to :doc:`forms created with Form Builder </user_guide/addons/form_builder/create_form>`. That's because the checkbox can be created via the Form Builder itself.

   In that case the consent for personal data processing won't be stored in the database, but rather in an email you receive, alongside the data that the customer may've provided via the form.

#. Test the workflow of granting consent. Register as a new customer and give consent for personal data processing in various places. If you completed :ref:`the optional step 2 <gdpr-data-request-buttons>`, try using the buttons for requesting personal data or the removal of data.

#. Open your database to see the consent logs in the ``cscart_gdpr_user_agreements`` table.

   .. image:: img/gdpr-database.png
       :align: center
       :alt: A table in the database that stores customers' consent for personal data processing.

#. As an administrator, try :doc:`exporting personal data and anonymizing a customer </user_guide/users/customers/gdpr>`.

   .. note::

       Customers would have to contact you to request their personal data or anonymization. For example, they can do it via email that you provide in the notices about personal data processing in step 2.

   .. image:: img/gdpr-user.png
       :align: center
       :alt: The personal data of a user in the admin panel.

======================================
Step 6. Make Sure You Comply with GDPR
======================================

**The add-on by itself won't make you GDPR-compliant.** We recommend `familiarizing yourself with the GDPR <http://eur-lex.europa.eu/legal-content/EN/TXT/?uri=uriserv:OJ.L_.2016.119.01.0001.01.ENG&toc=OJ:L:2016:119:TOC>`_ and looking into other measures that you may need to take.

For example, you may want to review and update your legal documents to address the requirements of the GDPR. For your online store, those documents could be:

* **Privacy Policy.** It exists by default under **Website → Pages** in the Administration panel, unless you have deleted it. You can edit it like any other content page in your store.

* **Terms of Service.** They appear at checkout if you *ask customers to agree to terms & conditions during checkout* under **Settings → Checkout**. The text can be edited under **Administration → Text & Languages → Edit texts** in the following language variable: ``terms_and_conditions_content``.
