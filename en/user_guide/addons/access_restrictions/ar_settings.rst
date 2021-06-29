***********************************
Access Restrictions Add-on Settings
***********************************

You can manage the following settings in the **Add-ons → Manage add-ons** section of the administration panel. Find the **Access restrictions** add-on, click on its name, and open the **Settings** tab.

Administrator area settings
***************************

The following parameters define access rules to the Administration panel.

*	**Allow login to the admin area from specified IPs only** — if selected, the administration panel can be accessed from a limited range of IP-addresses defined in the **Administration → Access restrictions** page.

.. important::

	When you enable this option, your current IP-address is automatically added to the list of allowed IP-addresses.

*	**Block IP after a number of unsuccessful attempts** — if selected, the system blocks the user IP-address after a series of failed login attempts made from this IP-address during a certain period of time. The number of attempts and the surveillance period are defined in the fields below.
*	**Number of unsuccessful attempts** — number of failed login attempts before the system blocks the IP-address.
*	**Time between unsuccessful login attempts** — number of seconds to include the series of failed login attempts after which the system blocks the IP-address.
*	**Time for which the IP should be blocked** — number of hours before the system unlocks a blocked IP-address.

When an administrator's IP is blocked, it appears among banned IP addresses in **Administration → Access restrictions** in the **Administration panel** tab having the *Active* status. Changing the status to *Disabled* unlocks the IP-address after the locking period is over.

Customer area settings
**********************

*	**Block IP after a number of unsuccessful attempts** — if selected, the system blocks the user IP-address after a series of failed login attempts made from this IP-address during a certain period of time. The number of attempts and the surveillance period are defined in the fields below.
*	**Number of unsuccessful attempts** — number of failed login attempts before the system blocks the IP-address.
*	**Time between unsuccessful login attempts** — number of seconds to include the series of failed login attempts after which the system blocks the IP-address.
*	**Time for which the IP should be blocked** — number of hours before the system unlocks a blocked IP-address.