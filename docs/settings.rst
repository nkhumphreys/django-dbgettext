.. _settings:

Settings
========

The following settings can be overridden in your project's ``settings.py``:

* ``DBGETTEXT_PATH``: path (absolute or relative to project root) where :doc:`dbgettext_export <dbgettext_export>` should store its output. Defaults to ``locale``.
* ``DBGETTEXT_ROOT``: name of directory within ``DBGETTEXT_PATH`` (redundancy to provide protection from auto-purging upon export). Defaults to ``dbgettext``.
* ``DBGETTEXT_REGISTRATION_MODULE_NAME``: name of modules within apps for registration. Defaults to ``dbgettext_registration``
* ``DBGETTEXT_PROJECT_OPTIONS``: dotted path to python module containing project-level registration code (e.g. ``my_project.dbgettext_options`` if you have a ``dbgettext_options.py`` file in your ``my_project`` directory).
* ``DBGETTEXT_INLINE_HTML_TAGS``: tuple of tag names allowed to appear inline within strings parsed with ``dbgettext.lexicons.html``. Defaults to ``('b','i','u','em','strong',)``.
* ``DBGETTEXT_SPLIT_SENTENCES``: split chunks of text into separate sentences for translation where appropriate. Defaults to ``True``.
* ``DBGETTEXT_SENTENCE_RE``: compiled regular expression for splitting sentences. Defaults to ``re.compile(r'^(.*?\S[\!\?\.])(\s+)(\S+.*)$', re.DOTALL)``.
