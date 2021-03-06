=====================================
Two Scoops of Django 1.8 Change List
=====================================

**Warning: This is a work in progress and may not match the current status of Two Scoops of Django 1.8.**

Two Scoops of Django 1.8 Change List Update #1
==============================================

* Chapter: Project Layout

  * Fixed URL to cookiecutters

* Chapter: Building REST APIs

  * In warning box about simple API lacking permissions, linked to relevant section in DRF documentation.

* Chapter: Tradeoffs Replacing Core Components

  * Added mention of CAP theorem to the fad table

* Chapter: User Model

  * Added `verbose_name` argument to `PositiveIntegerField`.
  
* Chapter: Third-Party Packages

  * For the purpose of clarity, switched from OSI to choosealicense.com for selecting licenses.
  
* Chapter: Testing

  * Added subsection 22.3.7 on *Testing for Failure*.
  
  * added section 22.10 for alternatives to `unittest`
  
    * pytest and pytest-django
    * nose and django-nose
  
* Chapter: Security

  * Added warning box that static media is not protected by ``SecurityMiddleware``.
  
  * Added PasswordInput variant suggestion for payment information entered in public venues.
  
* Chapter: Ask Questions

  * Removed broken link to the defunct planetdjango.org
  
* Appendix G: Security Settings Reference (NEW)

  * ALLOWED_HOSTS
  
  * CSRF_COOKIE_SECURE
  
  * DEBUG
  
  * MIDDLEWARE_CLASSES
  
  * SECRET_KEY
  
  * SECURE_PROXY_SSL_HEADER
  
  * SECURE_SSL_HOST
  
  * SESSION_COOKIE_SECURE
  
  * SESSION_SERIALIZER

* PDF TOC navbar now have chapter/section numbers
* Grammar/Spelling

Two Scoops of Django 1.8 Early Release Change List
==================================================

* General:

  * Bumped up version to Django 1.8 everywhere applicable

  * Various grammar mistakes have been corrected

  * Removed references to django.views.defaults.shortcut and django.conf.urls.shortcut
  
  * Moved lists of tables/figures to the back
  
  * Longer chapter, section, subsection and box titles now break more aesthetically on their pages.

* Introduction

  * Added clarity to section on Fat Models, Thin Views, Helper functions, and stupid templates

* Chapter: Coding Style

  * JS style guides
  
  * JS style checker packages
  
  * HTML/CSS style guides
  
  * CSS style checker packages

* Chapter: The Ultimate Django Environment Setup

  * Added virtalenvwrapper-win for windows
  
  * Merged in the chapter on Identical Environments

* Chapter: How to Lay Out Django Projects

  * Cookiecutter-django for default project layout
 
  * Use config for root config directory of project
  
  * Added Kevin Xu's fork of Two Scoops Project project.
  
* Chapter: Django apps

  * Explained conventions for naming modules
 
* Chapter: Models

  * Removed South mentions
  
  * Added content for django.db.migrations
  
  * Added Postgres fields
  
  * Recommended against use of generic relations. Truth: Great for the implementor, never ends well for the maintainer. :(
  
  * Lazy Evaluation!
  
  * Mentioned _meta
  
  * Discussed Fat models, how to make them and how to avoid the god class anti-pattern
  
  * Broke out queries and database interactions into their own chapter
  
* Chapter: Queries and the Database (NEW)

  * Added database functions
  
  * Added try/except issues and exceptions to use.

* Chapter: Function- and Class-Based Views

  *  Warned against use of dotted paths in URL definitions

* Chapter: Form Fundamentals (NEW)

  * Moved 'more forms' to be the basics of things to do with forms
  
  * Now explicitly instructing to use forms for all incoming data
  
  * Added mention of ModelForms for non-web data
  
  * Added mention fields without pre-made widgets
  
  * Moved some material from security chapter to this chapter

* Chapter: Forms and Class-Based Views

  * django.forms.Field.has_changed() instead of django.forms.Field._has_changed()
  
* Chapter: Templates

  * Mention use of Jinja2

* Chapter: Django and Jinja2

  * Using default filters in Jinja2
  
  * Replacing the need for context_processors with middleware.
  
  * Address CSRF usage.
  
  * The static nature of the Jinja2 Environment class.
  
* Chapter: Rest API

  * Added 410 methods
  
  * Mention Service-Oriented Architecture
  
  * Rate limiting APIs
  
  * Promoting your API
  
  * Create SDKs for API integrators
  
  * Some material on Service Oriented Architecture
  
* Consuming REST APIs (our kinda JavaScript chapter)

  * Remind the reader that JavaScripty stuff changes too fast.

  * Mention react
  
  * Switch from Grunt to Gulp

* Chapter: Admin

  * @admin.register decorator
  
  * Corrected our advice for __str__ or __unicode__.
  
* Chapter: Third-Party Packages

  * Pointed at Audrey's project release checklist
  
  * Advocate use of cookiecutter for jumpstarting projects
  
  * Suggested appveyor for getting Windows users of projects
  
* Chapter: Testing

  * Tricks for using Request Factory. Like example of request middleware having a session attached.
 
  * Quick intro to using Mock
 
  * Described integration tests
  
* Chapter: Documentation

  * Pandoc for converting long README.md to long README.rst

* Chapter: Bottleneckes

  * Added Silk profiling project
  
  * Recommended Lincoln Loop's High Performance Django

* Chapter: Security

  * Fix borked security link
  
  * Additional HSTS warnings
  
  * More warnings for Session cookies.
  
  * Mentioned Two-Factor Auth
  
  * Moved some content to forms chapter
  
* Chapter: Third Party Packages

  * Refactored how we describe broad version requirements
 
* Chapter: Utilities

  * Mentioned deprecation and danger of using remove_tags
  
  * Added awesome-slugify

* Chapter: Deployment

  * Added high level instructions for starting from scratch

  * Really, really don't use mod_python

  * Removed suggested practices for Salt and Ansible. They are out of scope for this book and the content changes too quickly.
  
* Chapter: Identical Environments

  * Merged into the The Ultimate Django Environment Setup chapter
  
* Chapter: Continuous Integration

  * Added AppVeyor
  
* Chapter: Debugging (new)

  * PDB/IPDB
  
  * Django-debug-toolbar: Just in case it isn't being used yet
  
  * Reminder about annoying ALLOWED_HOSTS in deployments
  
  * Common CBV error debugging trick

  * Context processor for debugging (thanks @simonw)
  
  * feature flags (again thanks @simonw)
  
* Appendix: Resources

  * Added new stuff

  * Removed stuff that is out of date
  
  
  
