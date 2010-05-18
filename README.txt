SMS Lox24 Modul
Mirko Haaser mcgo@drupalist.de

What?
-----
This module enables the SMS Framework to sent SMS via the Lox24 Gateway

How?
----
1. Create an account at www.lox24.eu and send some money to adjust your balance.
2. Install the SMS Framework module from http://drupal.org/project/smsframework
3. Drop this modul into a subdir of your choice (regarding the Drupal standards),
   for example sites/all/modules
4. Enable the module under admin/build/modules
5. Configure the module under admin/smsframework/gateways/lox24
   a. enter your account details that you created in Step 1
   b. enter a service id of your choise. You can get more information about this
      on the lox24.eu site.
   c. your information will be validate when you klick save. If you receive an
      error, it will hopefully give you further instruction on what to do.
6. Use the SMS Framework module or any other module that uses it (like messaging)

Common mistakes
---------------
- As far as I have seen, the gateway wants to have the target number in a format
  like 0049123987654 that is countrycode, area code, extension without any additional
  characters between.

Roadmap
-------
- The gateway send status info back, i think i might implement that
- The gateway allows one to get answer sms if you don't use your source identifier.
  The sms framework supports thie in a basic way, so i will implement that, too.

Support
-------
If you have any questions, please open an issue on http://drupal.org/node/add/project-issue/sms_lox
