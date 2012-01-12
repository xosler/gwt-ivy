# GWT-Ivy

This xml files will help you to create GWT apps and manage their dependencies with **Apache Ivy**.

## To do this, follow these steps:

1. Create a GWT project with your IDE or with the GWT-SDK;

2. Copy the build.xml, `ivy-setting.xml` and `ivy.xml` to the root of the project.

3. Alter build.xml to your prefered project name and module name. Basically, you need to change these lines by something like this:

`
project name="gwt-bree" xmlns:ivy="antlib:org.apache.ivy.ant" default="build" basedir="."
!-- some code --
   property name="application.module" value="com.geekvigarista.gwt.ivy.Gwt_bree" /
   property name="application.name" value="gwtbree" /
   !-- some code --
/project
`

In this example I changed the *gwt-ivy* default name by *gwt-bree*, thats also a real app managed by [gwt-bree](https://github.com/caarlos0/gwt-bree).

-----------------

## This is the basic config, now, will show you some commands:

1. `ant war` will do everything necessary and make a war in application root directory.
2. `ant libs` will download (if necessary) and copy all libs to a folder named *lib* in your root application diretory.

***TODO***


