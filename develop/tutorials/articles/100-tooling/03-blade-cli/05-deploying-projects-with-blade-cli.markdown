# Deploying Projects with Blade CLI [](id=deploying-projects-with-blade-cli)

Deploying projects to a Liferay server using Blade CLI is easy. To use
the Blade `deploy` command, you must first have built a project to deploy. See
the
[Creating Projects with Blade CLI](/develop/tutorials/-/knowledge_base/7-1/creating-projects-with-blade-cli)
tutorials for more information about creating Liferay projects. Once you've
built a project, navigate to it with your CLI and execute the following command
to deploy it:

    blade deploy

This can be used for WAR-style projects and modules (JARs). You can also deploy
all projects in a folder by running the `deploy` command from the parent folder
(e.g., `[WORKSPACE_ROOT]/modules`).

If you're using Liferay Workspace, the `deploy` command copies your project to
the @product@ `/deploy` folder, which is found by reading the Liferay Home
folder set in your workspace's `gradle.properties` file (i.e.,
`liferay.workspace.home.dir`). The `deploy` command works similarly if you're
working outside of workspace; the Liferay Home folder, in contrast, is set by
loading the Liferay extension object (Gradle) or the effective POM (Maven) and
searching for the Liferay Home property stored there. If it's not stored, Blade
prompts you to set it so it's available.

<!-- Above paragraph is explained based on how it was described BEFORE
development (BLADE-361). Follow up and update as necessary. -Cody -->

+$$$

**Note:** The `blade deploy` command requires a Gradle/Maven wrapper to
successfully execute. To ensure the availability of a build tool wrapper, work
in a Liferay Workspace. For more information on Liferay Workspaces, see the
[Creating a Liferay Workspace with Blade CLI](/develop/tutorials/-/knowledge_base/7-1/creating-a-liferay-workspace-with-blade-cli)
tutorial.

$$$

+$$$

**Note:** If you run into errors during the build/deploy process of your
project, check to make sure your workspace is accounting for the
[appropriate certificates](/develop/tutorials/-/knowledge_base/7-1/configuring-a-liferay-workspace#certification-issues-in-liferay-workspace).

$$$

You can also watch the deployed module for changes by specifying the `-w`
parameter.

    blade deploy -w

This parameter automatically redeploys the module when changes are detected.

Cool! You've successfully deployed your module project using Blade CLI.
