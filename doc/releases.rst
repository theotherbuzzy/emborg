Releases
========

**Latest development release**:
    | Version: 1.16.1
    | Released: 2020-04-12

**1.16 (2020-03-17)**:
    - refinements and bug fixes.

**1.15 (2020-03-06)**:
    - improve messaging from *emborg-overdue*
    - :ref:`configs <configs>` command now outputs default configuration too.
    - some commands now use first subconfig when run with a composite 
      configuration rather than terminating with an error.
    - added :ref:`show_stats` setting.
    - added ``--stats`` option to :ref:`create <create>`, :ref:`delete <delete>` 
      and :ref:`prune <prune>` commands.
    - added ``--list`` option to :ref:`create <create>`, :ref:`extract 
      <extract>` and :ref:`restore <restore>` commands.
    - added sorting and formatting options to :ref:`manifest <manifest>` 
      command.
    - added :ref:`manifest_formats` setting.
    - renamed ``--trial-run`` option to ``--dry-run`` to be more consistent with 
      *Borg*.
    - add *files* and *f* aliases to :ref:`manifest <manifest>` command.
    - added :ref:`working_dir` setting.
    - added :ref:`do_not_expand` setting.
    - added :ref:`exclude_nodump` setting
    - added :ref:`patterns` and :ref:`patterns_from` settings.
    - *Emborg* lock file is now ignored if the process it references is no 
      longer running
    - support ``--repair`` option on :ref:`check command <check>`.

**1.14 (2019-12-31)**:
    - remove debug message accidentally left in *emborg-overdue*

**1.13 (2019-12-31)**:
    - enhance *emborg-overdue* to work on clients as well as servers

**1.12 (2019-12-25)**:
    - added :ref:`default_mount_point` setting.
    - fixed some issues with :ref:`borg <borg>` command.
    - added ``--oldest`` option to :ref:`due <due>` command.

**1.11 (2019-11-27)**:
    - Bug fix release.

**1.10 (2019-11-11)**:
    - Bug fix release.

**1.9 (2019-11-08)**:
    - Added ability to check individual archives to the :ref:`check <check>` command.
    - Made latest archive the default for :ref:`check <check>` command.
    - Allow :ref:`exclude_from <exclude_from>` setting to be a list of file 
      names.

**1.8 (2019-10-12)**:
    - Remove duplicated commands.

**1.7 (2019-10-07)**:
    - Fixed bug that involved the Boolean Borg settings
      (:ref:`one_file_system <one_file_system>`, :ref:`exclude_caches <exclude_caches>`, ...)

**1.6 (2019-10-04)**:
    - Added :ref:`restore <restore>` command.
    - Added :ref:`verbose <verbose>` setting.

**1.5 (2019-09-30)**:
    - Added composite configurations.
    - Added support for multiple backup configurations in a single repository.
    - Added :ref:`prefix <prefix>` and :ref:`exclude_from <exclude_from>` 
      settings.
    - Provide default value for :ref:`archive <archive>` setting.
    - Add --all command line option to :ref:`mount <mount>` command.
    - Add --include-external command line option to :ref:`check <check>`, :ref:`list <list>`, 
      :ref:`mount <mount>`, and :ref:`prune <prune>` commands.
    - Add --sort command line option to :ref:`manifest <manifest>` command.
    - Add --latest command line option to :ref:`delete <delete>` command.
    - Added --quiet command line option
    - :ref:`umount <umount>` command now deletes directory used as mount point.
    - Moved log files to ~/.local/share/emborg
      (run 'mv ~/.config/emborg/\*.{log,lastbackup}\* ~/.local/share/emborg' 
      before using this version).

**1.4 (2019-04-24)**:
    - Added *ssh_command* setting
    - Added --fast option to :ref:`info <info>` command
    - Added *emborg-overdue* executable
    - Allow :ref:`run_before_backup <run_before_backup>` and :ref:`run_after_backup <run_after_backup>` to be simple 
      strings

**1.3 (2019-01-16)**:
    - Added the raw :ref:`borg <borg>` command.

**1.2 (2019-01-16)**:
    - Added the :ref:`borg_executable <borg_executable>` and :ref:`passcommand <passcommand>` settings.

**1.1 (2019-01-13)**:
    - Improved and documented API.
    - Creates the settings directory if it is missing and add example files.
    - Added --mute command line option.
    - Support multiple email addresses in :ref:`notify <notify>`.
    - Added warning if settings file is world readable and contains a passphrase.

**1.0 (2019-01-09)**:
    - added :ref:`remote_path <remote_path>` setting.
    - formal public release.

**0.3 (2018-12-25)**:
    - initial public release (beta).

**0.0 (2018-12-05)**:
    - initial release (alpha).
