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
folder set in your workspace's `gradle.properties` or `pom.xml` file. The
`deploy` command works similarly if you're working outside of workspace; the
Liferay Home folder, in contrast, is set by loading the Liferay extension object
(Gradle) or the effective POM (Maven) and searching for the Liferay Home
property stored there. If it's not stored, Blade prompts you to set it so it's
available.

+$$$

**Note:**

If you prefer using pure Gradle or Maven to deploy your project, you can do this
by applying the appropriate plugin and configuring your Liferay Home property.
Here's how you can do this for Gradle and Maven:

**Gradle:**

First ensure the Liferay Gradle plugin is applied in your `build.gradle` file:

    apply plugin: "com.liferay.plugin"

Then extend the Liferay extension object to set your Liferay Home and `deploy`
folder:

    liferay {
        liferayHome = "../../../../liferay-ce-portal-7.1.1-ga2"
        deployDir = file("${liferayHome}/deploy")
    }

**Maven:**

Ensure the Bundle Support plugin is applied and configure Liferay Home in your
`pom.xml`. See the
[Deploying a Project Built with Maven to Liferay Portal](/tutorials/-/knowledge_base/7-1/deploying-a-project-built-with-maven-to-product)
for details.

$$$

Cool! You've successfully deployed your module project using Blade CLI.
