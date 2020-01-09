[//]: # (title: First Failure)
[//]: # (auxiliary-id: First Failure)
TeamCity displays the "First Failure" build for some tests.

This is the build where TeamCity detected the first failure of this test for the same [Build Configuration](build-configuration.md), which means that starting from the current build, TeamCity goes back throughout the build history to find out when this test failed for the first time. Builds without this test are skipped, and if a successful test run was found, the search stops.

"Back throughout the history" means that builds are analyzed with regard to changes as detected by TeamCity, i.e. [History Build](history-build.md)s will be processed correctly.

A test which is run several times within a single build is counted as one test (i.e. all invocations of the same test are counted as 1).

<seealso>
        <category ref="concepts">
            <a href="already-fixed-in.md">Already Fixed In</a>
        </category>
</seealso>