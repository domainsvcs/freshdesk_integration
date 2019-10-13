CONTENTS OF THIS FILE
---------------------

 * Introduction
 * Requirements
 * Recommended modules
 * Installation
 * Configuration
 * Maintainers


INTRODUCTION
------------

Freshdesk Integration aims to provide a tight, API-based integration allowing
your site to push and sync users and user information such as profile photos
and roles (stored in Freshdesk as Companys) to your Freshdesk account.

 * For a full description of the module, visit the project page:
   https://www.drupal.org/project/freshdesk_integration

 * To submit bug reports and feature suggestions, or to track changes:
   https://www.drupal.org/project/issues/freshdesk_integration


REQUIREMENTS
------------

You must have an active Freshdesk account (https://freshdesk.com/) and be able
to create an API key under a sufficiently privileged user within Freshdesk.


RECOMMENDED MODULES
-------------------

 * This module has no dependencies for normal use.  Some included utility
   functions intended only for developers can be called from the Devel module.

INSTALLATION
------------

 * Install as you would normally install a contributed Drupal module.
   See: https://www.drupal.org/node/895232 for further information.


CONFIGURATION
-------------

 * Configuration is located under
   Configuration > Web services > Freshdesk Integration, or
   /admin/config/services/freshdesk_integration
 
 * Most configuration is self-explanatory, except for "Map roles to Freshdesk
   Companies".  According to Freshdesk support, Freshdesk does not support user
   roles for providing access to Knowledge-base resources within your Freshdesk
   portal.  The suggested solution is to create the Roles as Companies within
   their system, and use the Company field to manage access.  We implemented
   their suggestion by providing a way for admins to associate Drupal "Roles"
   with Freshdesk "Companies" on the configuration page.  When a user is
   created or updated within Freshdesk by Drupal, the associated role will be
   assigned as a company within Freshdesk.  Currently, due to limitations in
   the Freshdesk system, only one Company may be associated with a Freshdesk
   user, so only one field should be filled in this configuration table.
   
   We created this as a table for possible future use.  If necessary we may
   change this to a set of dropdown selects.


MAINTAINERS
-----------

Current maintainers:
 * Randall Box (rbox) - https://www.drupal.org/u/rbox

This project has been sponsored by:
 * Ion Agency
   Founded in 2005, Ion Agency supports the open web by designing, developing,
   and implementing solutons for large and small organizations utilizing open
   source technology, contributing back advancements made along the way.
