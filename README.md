nrser.iterm
===========

install iterm from homebrew cask and configure.

Requirements
------------

Ruby

Role Variables
--------------

-   `iterm_control_backtick_visor`
    -   set to `yes` use cmd+` to open visor
    -   *default:* `no`

-   `iterm_prompt_on_quit`
    -   prompt when quitting iterm

-   `iterm_no_windows_on_start`
    -   set to `yes` to not show any windows on iTerm start
        (visor will open with ctrl+` when enabled)
    -   *default:* `no`

-   `iterm_silence_bells`
    -   silence the bells on all profiles.
    -   *default:* `no`

Dependencies
------------

-   nrser.state_mate
-   nrser.sync.rb

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
      - role: nrser.iterm
        iterm_control_backtick_visor: yes
        iterm_prompt_on_quit: false
        iterm_no_windows_on_start: yes
        iterm_silence_bells: yes

License
-------

BSD

Author Information
------------------

<https://github.com/nrser>
