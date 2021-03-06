Customers and Users
===================

Users
~~~~~

Creating a User
^^^^^^^^^^^^^^^

1. Navigate to the Users admin page by clicking `Users` under the
   `Settings` category from the Shuup Admin menu.
2. Click the `New User` button on the Users admin toolbar.

   .. image:: customers-and-users/new-user-button.png

3. Enter a valid username and password for the user as well as any
   other user information, including the `Staff User` checkbox. A Staff user 
   has the ability to login in the admin panel.
   
4. Then click the `Save` button in the
   to create the user account.

   .. image:: customers-and-users/new-user.png

.. note::
   Unless they have a `Staff status` and the `Send email confirmation` 
   box is checked, a user won't automatically receive notice that 
   an account has been created for them.

   Instead, if you would like to notify a user, send a password-reset
   email.

   See `Sending Password-Reset Emails`_.

Creating a User From a Saved Contact
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Navigate to the Contacts admin page by clicking `Contacts` under the
   `Contacts` category from the Shuup Admin menu.

   .. image:: customers-and-users/contacts-menu.png

2. Select the contact for which you want to create a user account.

   .. image:: customers-and-users/select-contact.png

3. Click the `Options` button on the Contact admin toolbar and select `New User`.

..   .. image:: customers-and-users/new-user-from-contact.png

4. Enter the new user's username and password information and click
   `Save` to create the user account, which will now be associated with
   the selected contact information.

   .. image:: customers-and-users/new-user.png


   See `Creating a User`_ for more information.

Managing User Passwords
^^^^^^^^^^^^^^^^^^^^^^^

Changing User Passwords
***********************

1. Navigate to the Users admin page by clicking `Users` under the
   `Settings` category from the Shuup Admin menu.

   .. image:: customers-and-users/users-menu.png

2. Select the user whose password you want to change.

   .. image:: customers-and-users/select-user.png

3. Click the `Actions` button on the user admin toolbar and select
   `Change Password` from the dropdown menu.

   .. image:: customers-and-users/change-password.png

4. Enter the current and new passwords in the `Change User Password` 
   form and click `Save` in the toolbar to save the new password.

..   .. image:: customers-and-users/change-password-form.png

Sending Password-Reset Emails
*****************************

1. Navigate to the Users admin page by clicking `Users` under the
   `Settings` category from the Shuup Admin menu.

   .. image:: customers-and-users/users-menu.png

2. Select the user whose password you want to change.

   .. image:: customers-and-users/select-user.png

3. Click the `Actions` button on the user admin toolbar and select
   `Send Password Reset Email` from the dropdown menu.

   .. image:: customers-and-users/send-password-reset-email.png

4. On the next screen, click `Send Reset Email` to send the user a
   password reset email.

   .. image:: customers-and-users/send-reset-email.png

Editing User Permissions
^^^^^^^^^^^^^^^^^^^^^^^^

.. warning::

   Use caution when granting users administrative permissions.

1. Navigate to the Users admin page by clicking `Users` under the
   `Settings` category from the Shuup Admin menu.
2. Select the user whose permissions you want to edit.
3. Click the `Actions` button on the user admin toolbar and select
   `Edit Permissions` from the dropdown menu.

   .. image:: customers-and-users/edit-permissions.png

4. Check the permission levels that want to grant the user and click
   the `Save` button to save the user's permissions.

   .. image:: customers-and-users/change-permissions.png

See `Permission Groups`_ for more information on how to create and manage
Permission Groups.

Deactivating a User
^^^^^^^^^^^^^^^^^^^

When users are deactivated, they remain in your system however they
will no longer be able to log in to their account and by default are
not displayed when first opening the Users admin page.

.. note::
   If a user has an associated contact, deactivating the user's user
   account will not deactivate their contact, although it will prevent
   them from logging in, essentially accomplishing the same thing.

   See `Deactivating a Contact`_ for more information.

To deactivate a user:

1. Navigate to the Users admin page by clicking `Users` under the
   `Settings` category from the Shuup Admin menu.

   .. image:: customers-and-users/users-menu.png

2. Select the user you want to deactivate.

   .. image:: customers-and-users/select-user.png

3. Click the `Deactivate User` button on the user admin toolbar.

   .. image:: customers-and-users/deactivate-user-button.png

4. The user will now be deactivated, and the `Deactivate User` button
   will be replaced with an `Activate User` button.

.. note:: The same steps can be followed to activate a deactivated user.

.. _`Permission Groups`:

Permission Groups
~~~~~~~~~~~~~~~~~

Permission groups can be used to restrict access to different sections
of the Shuup admin for staff-level users. Superusers have unrestricted 
access to any section.

Creating a Permission Group
^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Navigate to the Permission Groups admin page by clicking `Permission
   Groups` under the `Shops` category from the Shuup Admin menu.
2. Click the `Create New Permission group` button on the Permission 
   Group admin toolbar.
3. Enter a name for the group, select any users that should be
   members of this group. You can also set the group for a user while 
   editing it.
   
   .. image:: customers-and-users/new-group.png
   
4.  go through all the permissions sections and check the features you want 
to give permission.

   .. image:: customers-and-users/permissions.png


.. note::

      On every permission section, you will see `Module permission` and 
      `Features permissions`. If you give the `Module permission`, it will tell 
      to Shuup that the user can access the module as a whole. Users will be 
      able to access the module through the main menu for example. 
      
      You can also give specific features permissions that will enable users to 
      create, delete, list objects and other features that the module provides. 
      You can give permission for the features and have the `Module permission` 
      disabled at the same time. Disabling the module permission won't interfere 
      on the feature permission as they are complements of each other. 
      
      One example for this is when you want to allow users to create customers 
      while they are creating an order, but you don’t want them to access the 
      customer list through the main menu. On this case you disable the customer 
      module permission and enable the customer edit feature permission.

      .. image:: customers-and-users/multi-select-permissions.png

The buttons `Select all permissions` and `Deselect all permissions` will check or 
uncheck all the permissions which can be helpful when you want to disable just a 
few permissions for the user. 

5. Click `Save` to save the permission group settings.

See `Editing User Permissions`_ for more information on how to set specific 
permissions for a single User.

Contacts
~~~~~~~~

Shuup contacts store contact information such as address data, email, or
phone numbers, and a contact may or may not be associated with a
user account.

Contacts may be one of the two following types:

Person contact
   Contact associated with a person.
Company contact
   Contact associated with a company.

One or more person contacts may be *members* of a company contact.

However, if a user has a contact associated with their account, it must
always be a *person*-type contact, which may then be a member of one or
more *company* contacts.

If a user's person contact is linked to a company, the company's contact
information will be used when placing orders.

Creating a Contact
^^^^^^^^^^^^^^^^^^

1. Navigate to the Contacts admin page by clicking `Contacts` under the
   `Contacts` category from the Shuup Admin menu.

   .. image:: customers-and-users/contacts-menu.png

2. Click the `New Person` or the `New Company` button on the Contacts 
   admin toolbar.

..   .. image:: customers-and-users/new-contact-button.png

3. Enter all basic details for the contact, including any required
   fields.

   .. image:: customers-and-users/contact-basic-details.png

4. Click the `Save` button to create the contact.

Editing a Contact
^^^^^^^^^^^^^^^^^

1. Navigate to the Contacts admin page by clicking `Contacts` under the
   `Contacts` category from the Shuup Admin menu.

   .. image:: customers-and-users/contacts-menu.png

2. Select the contact that you want to edit.

   .. image:: customers-and-users/select-contact.png

3. Click the `Edit` button in the contact admin toolbar.

   .. image:: customers-and-users/edit-contact.png

4. Edit the user's information.

5. Click the `Addresses` tabs on the left-hand side of the screen to
   enter billing and shipping address information for the contact.

   .. image:: customers-and-users/contact-addresses.png

6. Click `Save` to save the contact's information.

   See `Creating a Contact`_ for more information.

Editing Company Membership
^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Navigate to the Contacts admin page by clicking `Contacts` under the
   `Contacts` category from the Shuup Admin menu.

   .. image:: customers-and-users/contacts-menu.png

2. Select the company contact whose membership you want to edit.

   .. image:: customers-and-users/select-company.png

3. Click the `Edit` button in the contact admin toolbar.

   .. image:: customers-and-users/edit-contact.png

4. Under the `Members` field input, type the name of the person contact
   you wish to add to the company. When the name appears in the
   dropdown, click to add to the input field.

   .. image:: customers-and-users/company-membership.png

5. Click save to update the company's memberships.

Creating a Contact From a User Account
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1. Navigate to the Users admin page by clicking `Users` under the
   `Settings` category from the Shuup Admin menu.

   .. image:: customers-and-users/users-menu.png

2. Select the user whose permissions you want to edit.

   .. image:: customers-and-users/select-user.png

3. Click the `Actions` button on the user admin toolbar and select
   `Create Contact` from the dropdown menu.

   .. image:: customers-and-users/new-contact-from-user.png

4. Fill in the user's contact information, including any required
   fields, then save to create a saved contact for the user.

..   .. image:: customers-and-users/contact-basic-details.png

   See `Creating a Contact`_ for more information.

5. The contact will now be created and you will be taken to the new
   contact's admin page.

   Click the user's username to go back to the user's admin page.

Deactivating a Contact
^^^^^^^^^^^^^^^^^^^^^^

When contacts are deactivated, they remain in your system however they
will no longer be able to log in to their account and by default are
not displayed when first opening the Contacts admin page.

.. note::
   If a contact has an associated user, deactivating the user's contact
   will not deactivate their user account, although it will prevent them
   from logging in, essentially accomplishing the same thing.

   See `Deactivating a User`_ for more information.

To deactivate a contact:

1. Navigate to the Contacts admin page by clicking `Contacts` under the
   `Contacts` category from the Shuup Admin menu.

   .. image:: customers-and-users/contacts-menu.png

2. Select the contact you want to deactivate.

   .. image:: customers-and-users/select-contact.png

3. Click the `Deactivate Contact` button on the contact admin toolbar.

   .. image:: customers-and-users/deactivate-contact-button.png

4. The contact will now be deactivated, and the `Deactivate Contact`
   button will be replaced with an `Activate Contact` button.

.. note::
   The same steps can be followed to activate a deactivated
   contact.

Contact Groups
~~~~~~~~~~~~~~

In Shuup, contacts can be placed into different contact groups. These
groups can then be targetted for campaigns, discount pricing, or custom
behaviors.

.. Add information about default groups

Creating a Contact Group
^^^^^^^^^^^^^^^^^^^^^^^^

1. Navigate to the Contact Groups admin page by clicking `Contact
   Groups` under the `Contacts` category from the Shuup Admin menu.

   .. image:: customers-and-users/contacts-menu.png

2. Click the `Create new` button in the Contact Groups toolbar.


   .. image:: customers-and-users/new-contact-group-button.png

3. Select a name for your contact group.

..   .. image:: customers-and-users/contact-group-information.png

4. Click the `Save` button to save your contact group.

   Once the contact group has been saved, two new tabs will be
   automatically added to the group's admin page--a `Members` tab
   and one or more `Sales Range` tabs.

Editing Group Membership
^^^^^^^^^^^^^^^^^^^^^^^^

View Contact Group Membership
*****************************

Adding a Contact
****************

1. Navigate to the Contact Groups admin page by clicking `Contact
   Groups` under the `Contacts` category from the Shuup Admin menu.

   .. image:: customers-and-users/contact-groups-menu.png

2. Select the contact group whose membership you want to edit.

   .. image:: customers-and-users/select-contact-group.png

3. Click the `Add Members` tab on the left-hand side of the screen.

   .. image:: customers-and-users/add-members-tab.png

4. Click the `Select Contact` button on an empty row to launch the Contact
   selector popup.

..   .. image:: customers-and-users/add-members-select-button.png

5. Select the contact you want to add from the Contact popup selector.

   .. image:: customers-and-users/select-member.png

5. If there are no blank contact rows, click the `Add more` button to
   add a blank contact row.

..   .. image:: customers-and-users/add-more-button.png

6. Repeat as necessary to add more contacts, then click `Save` to save
   the contact group.

Removing a Contact
******************

.. note::
   Contacts can only be removed from a contact group via the
   admin page for each contact you wish to remove.

1. Navigate to the Contacts admin page by clicking `Contacts` under the
   `Contacts` category from the Shuup Admin menu.

   .. image:: customers-and-users/contacts-menu.png

2. Select the contact that you want to remove from your group.

   .. image:: customers-and-users/select-contact.png

3. Click the `Edit` button in the contact admin toolbar.

..   .. image:: customers-and-users/edit-contact-group-from-contact.png

4. Find the contact group whose membership you wish to edit in the
   `Contact Groups` list, click the `x` button on the contact group, and 
   click `Save` to update the contact's group membership.

Creating a Sales Range
^^^^^^^^^^^^^^^^^^^^^^

Contact group *sales ranges* can be used to automatically assign
customer contacts to contact groups based on their sales totals.

This can be useful if you want to target different sales levels for
special campaigns or offer special discounts or promotions.

1. Navigate to the Contact Groups admin page by clicking `Contact
   Groups` under the `Contacts` category from the Shuup Admin menu.

   .. image:: customers-and-users/contact-groups-menu.png

2. Select the contact group to which you want to add a sales range.

   .. image:: customers-and-users/select-contact-group.png

3. Click the `(Shop Name) - Sales Ranges` tab on the left-hand side of
   the screen, where `(Shop Name)` is the name of the shop to associate
   with the sales range.

   .. image:: customers-and-users/sales-ranges-tab.png

4. Enter a minimum and maximum value for the group's sales range.

   .. image:: customers-and-users/sales-ranges-values.png

   .. note::

      Leave the maximum value blank to set no maximum for the group.

      Set the minimum value to 0 to set no minimum for the group.

5. Click `Save` to save the contact group sales range. Contact group
   membership will automatically update based on customers' sales
   totals.


.. tip::
   Try creating a contact group for customers within a sales range
   value and target them for special discounts and promotions.
