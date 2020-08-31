# About Craft Nitro

Nitro is a speedy local development environment tuned for [Craft CMS](https://craftcms.com/), powered by [Multipass](https://multipass.run/).

## What’s Included

Nitro installs the following on every machine:

- PHP 7.4 (+ option to use 7.3 or 7.2)
- MySQL
- PostgreSQL
- Redis
- Xdebug
- Blackfire
- MailHog

## System Requirements

- macOS, Linux, or Windows 10 Pro with Hyper-V enabled
- [Multipass](https://multipass.run/) 1.4.0+

## Overview

### Why Use Nitro?

- You work modern PHP apps like Craft CMS that may also need MySQL or PostgreSQL.
- It’s lovingly developed and supported by the Craft CMS team.
- It comes ready with useful tools like Xdebug and MailHog.
- Its only dependency is Multipass, meaning quick setup, isolated software (not installed directly on your system), and good performance.
- It’s free and cross-platform.

### Why Not Use Nitro?

- You’d prefer to manage local development sites with a GUI.
- You have older projects (PHP 5.6, 7.0, or 7.1) Nitro doesn’t support.
- You staunchly prefer IIS.

### How’s it compare with…?

#### MAMP Pro/WAMP/XAMPP

These popular packages bundle software binaries with a GUI for configuration.

Nitro installs software in a virtualized Ubuntu machine, configured via CLI and YAML. If you’ve ever worked with a VPS from a hosting provider, Nitro should feel similar. (Which could be good or bad, depending on your level of comfort!)

Ultimately Nitro’s virtualization may make it less performant than these options, but its configuration will be much more similar to a production hosting environment and easier to customize if your web server needs additional software.

#### Laravel Homestead

Laravel Homestead is an excellent, flexible option for local PHP development and Nitro should feel very similar to it in many ways. Nitro’s leaner focus makes it more performant and quicker to set up if you’re working with modern Craft projects.

#### Laravel Valet

Laravel Valet runs with native speed because it uses native software; each part of the web stack is installed directly on your system.

We prefer Nitro’s virtualization (via Multipass): development environments _should be_ ephemeral because your host OS is not. It’s much simpler and quicker to destroy and rebuild a web server than it is to wipe and reinstall your primary OS.

Another benefit is that Nitro offers the ability to create as many development machines as you’d like, each with the software and settings you choose.

#### DDEV/Lando

Docker-based development environments like DDEV and Lando can offer a nice balance of performance, flexibility, and portability. Nitro’s focus on Craft CMS and modern PHP should translate into more streamlined setup and fewer features you *aren’t* using.
