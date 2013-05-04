# Redmine own time entries

Plugin which allow to setup project permisions to show own time entries to user


## Redmine version

Version 1.4.0-stable


## Installation

Put plugin to the folder REDMINE/vendor/plugins, name directory as redmine_own_time_entries and restart Redmine

```bash
cd REDMINE/vendor/plugins
git clone https://github.com/Belarus2012/SelfSpentTime.git redmine_own_time_entries
```

No migrations, no new gems.


## Usage

Setup role permission "View only own time entries" to allow user see only own time entries


## Changes

Patches:
  * ApplicationController.authorize
  * ProjectsController.show
  * Project.allowed_to_condition
  * Issue#total_spent_hours
