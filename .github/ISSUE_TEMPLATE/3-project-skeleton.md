---
name: 🏗 Project Skeleton
about: "Capture advance requirements for a project's skeleton"
title: ""
labels: ["feature", "skeleton"]
assignees: ""
projects: ["hcsolutions/3"]
---

**Project:** #
<!-- **Prerequisites**: # -->

## Requirements
### Structure
<!-- What is/are the namespace(s)? -->
<!-- What are the tables, columns and datatypes required by this project? What are the accepted values for any enum fields? -->
<!-- Which columns need to be indexed, or cannot be NULL? -->
**Namespace:** 
```ruby
create_table :foos, id: :uuid do |t|
  t.uuid :id, default: -> { "gen_random_uuid()" }, null: false
  t.references :tenant, null: false, index: false
  t.references :site, type: :uuid, null: false
  t.string :name

  t.timestamps

  t.index :id
end
```

### Concerns
<!-- Which Concerns do the models created by this issue need to include? etc. -->

### Associations
<!-- How do these tables relate to each other and existing tables? e.g. `has_many`, `belongs_to` -->

### Routes
<!-- Provide details of which routes will be required. -->
<!-- This does not need to be exhaustive - routes can be added by later issues or left to engineer discretion. -->
<!--
index
_new
create
_edit
update
remove
restore
destroy
-->

<!-- Miscellaneous Additional Requirements -->
<!-- Add any additional heading you feel necessary e.g. ## Callbacks, ## Methods etc -->

### Populus <!-- Optional -->
<!-- Are there any examples of test/development data which we know already would be useful to include? -->

## Further Context <!-- Optional -->
<!-- Quotes from business SMEs, discussion transcripts etc. -->

