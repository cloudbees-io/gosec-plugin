= CloudBees action: Scan with Gosec

Use this action to perform static application security testing (SAST) on a repository with the Gosec scanner.

== Inputs

[cols="2a,1a,1a,3a",options="header"]
.Input details
|===

| Input name
| Data type
| Required?
| Description


| `ref`
| String
| No
| Specify the ref that should be checked out and archived.

| `workspace-dir`
| String
| No
| Specify the path where the checked out code will be present for scanning.

|===

== Usage example

In your YAML file, add:

[source,yaml]
----

      - name: Scan with Gosec
        uses: https://github.com/cloudbees-io/gosec-plugin@v1
        with:
          ref: main

----

== License

This code is made available under the 
link:https://opensource.org/license/mit/[MIT license].

== References

* Learn more about link:https://docs.cloudbees.com/docs/cloudbees-platform/latest/actions[using actions in CloudBees workflows].
* Learn about link:https://docs.cloudbees.com/docs/cloudbees-platform/latest/[the CloudBees platform].


