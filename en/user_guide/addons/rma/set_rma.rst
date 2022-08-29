*****************************
How To: Set up the RMA Add-on
*****************************

.. contents::
    :backlinks: none
    :local:

=======================
Enabling the RMA Add-on
=======================

#. In the Administration panel, go to **Add-ons → Manage add-ons**.

#. The **RMA** add-on is installed by default. If it is inactive (it's status is *Disabled*), change the add-on status to *Active*.

#. Click on the name of the **RMA** add-on.

#. Select the desired settings and tick the check boxes, if needed:

   .. note:: 

        The following settings are available in the CS-Cart and Multi-Vendor 4.15.2 and higher. After you set the settings, all new products will have the values of these settings by default.

        * **Refundable** — if selected, customers are able to return products.

        * **Return period (days)** — enter the number of days during which a customer is able to return a product.

   * **Display product return period** — if selected, product return period is displayed on the storefront.

   * **Do not take weekends into account when calculating product return period** — if selected, Saturdays and Sundays are excluded from the return period.

#. Click **Save**.

   .. image:: img/rma_01.png
       :align: center
       :alt: RMA add-on

==============================
Setting Up Return Registration
==============================

#. Go to **Orders → Return requests**.

#. Click the gear button in the top right corner of the page and choose **RMA reasons**.

#. Click the **+** button and create a reason why a customer will be able to return products.

   .. image:: img/rma_02.png
       :align: center
       :alt: RMA reasons

#. Click the gear button in the top right corner and choose **RMA actions**. Change the **Status** of the actions to *Active*.
 
#. Click **Save**.

   .. image:: img/rma_03.png
       :align: center
       :alt: RMA actions

#. Go to **Administration → Statuses → Order statuses**.

#. Click on the order status for which you want to allow return and tick the **Allow return registration** check box.

#. Click **Save**.

   .. image:: img/rma_04.png
       :align: center
       :alt: Allow return registration

============================
Editing RMA Request Statuses
============================

#. In the Administration panel go to **Administration → RMA request statuses**.

#. Choose whether you want to:

   * create a new status by clicking the **+** button;

   * edit an existing status by clicking its name;

   * use drag & drop to sort statuses.

#. Specify the status properties.

#. Click the **Create** or **Save** button.

   .. image:: img/rma_07.png
       :align: center
       :alt: RMA statuses
