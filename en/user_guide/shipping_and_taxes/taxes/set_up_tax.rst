********************
How To: Set up a Tax
********************

.. contents::
   :backlinks: none
   :local:

=================
Create Rate Areas
=================

Go to **Administration → Shipping & taxes → Rate areas** and :doc:`create rate areas </user_guide/shipping_and_taxes/locations/set_location>`. You'll need rate areas if you want to specify different tax rates for customers from different countries and regions.

===============
Configure a Tax
===============

#. Go to **Administration → Shipping & taxes → Taxes**.

#. Add a new tax by clicking the **+** button in the upper right part of the page, or edit an existing tax by clicking on it's name. 

#. The tax editing page will open. Specify :doc:`tax properties <tax_attributes>` there.

   .. image:: img/set_tax_01.png
       :align: center
       :alt: The tax editing page in CS-Cart and Multi-Vendor.

#. Switch to the **Tax rates** tab and enter the tax rates.

#. Click the **Save** button (or **Create** if you're adding a new tax).

   .. image:: img/set_tax_02.png
       :align: center
       :alt: Tax rates

   .. hint::

      Check **Settings → Appearance** for 2 settings related to taxes: 

      * Display prices with taxes on category/product pages

      * Display prices with taxes on cart/checkout pages

=======================
Apply Taxes to Products
=======================

.. important::

    If you want to apply several taxes to the base product price, make sure those taxes have the same priority. Otherwise, if the priority of **tax A** is *1* and the priority of **tax B** is *2*, the tax A will be applied to the base product price, and tax B will be applied to the product price with tax A applied already.

---------------------------
Apply Taxes to All Products
---------------------------

#. Go to **Administration → Shipping & taxes → Taxes**. 

#. Click the tax ot taxes that you want to apply to all products. Three sections with with drop-down settings that you can change for the selected taxes will appear.

#. Click the **Actions** button and choose **Apply selected taxes to all products**.

   .. image:: img/set_tax_03.png
       :align: center
       :alt: Apply a tax to all products in CS-Cart or Multi-Vendor.

---------------------------------
Apply Taxes to a Specific Product
---------------------------------

#. Go to **Products → Products**.

#. Find the product and click on its name.

#. Find the **Taxes** property in the **Pricing / inventory** section.

#. Tick the checkboxes of the taxes you'd like to apply.

#. Click **Save**.

   .. hint::

       Taxes can also be applied to products via :doc:`product_import </user_guide/manage_products/import_export/product_import>`. We have a separate article that describes :doc:`the formatting of the imported CSV file with products </user_guide/manage_products/import_export/fields_format>`.

===============================
Apply Taxes to Shipping Methods
===============================

#. Go to **Administration → Shipping & taxes → Shipping methods**. 

#. Click on the name of the shipping method.

#. Find the **Taxes** property in the **Pricing** section on the *Additional settings* tab.

#. Tick the checkboxes of the taxes you'd like you apply.

#. Click the **Save** button.

   .. image:: img/set_tax_04.png
       :align: center
       :alt: Applying a tax to a shipping method in CS-Cart or Multi-Vendor.
