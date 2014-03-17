maven-duplicate-gav
===================

Output from Apache Maven v3.1.1

    ➜  maven-duplicate-gav git:(master) mvn311 
    [INFO] Scanning for projects...
    [ERROR] Two or more projects in the reactor have the same identifier, please make sure that <groupId>:<artifactId>:<version> is unique for each project: {org.apache.maven:mod1:1-SNAPSHOT=[/misc/workspaces/jlf/apache/maven-duplicate-gav/mod1/pom.xml, /misc/workspaces/jlf/apache/maven-duplicate-gav/mod2/pom.xml]} -> [Help 1]
    [ERROR] 
    [ERROR] To see the full stack trace of the errors, re-run Maven with the -e switch.
    [ERROR] Re-run Maven using the -X switch to enable full debug logging.
    [ERROR] 
    [ERROR] For more information about the errors and possible solutions, please read the following articles:
    [ERROR] [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/DuplicateProjectException

Output from Apache Maven v3.2.1

    ➜  maven-duplicate-gav git:(master) ✗ mvn321 
    [INFO] Scanning for projects...
    [ERROR] Internal error: java.lang.NullPointerException -> [Help 1]
    org.apache.maven.InternalErrorException: Internal error: java.lang.NullPointerException
            at org.apache.maven.DefaultMaven.execute(DefaultMaven.java:167)
            at org.apache.maven.cli.MavenCli.execute(MavenCli.java:584)
            at org.apache.maven.cli.MavenCli.doMain(MavenCli.java:213)
            at org.apache.maven.cli.MavenCli.main(MavenCli.java:157)
            at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
            at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:57)
            at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
            at java.lang.reflect.Method.invoke(Method.java:606)
            at org.codehaus.plexus.classworlds.launcher.Launcher.launchEnhanced(Launcher.java:289)
            at org.codehaus.plexus.classworlds.launcher.Launcher.launch(Launcher.java:229)
            at org.codehaus.plexus.classworlds.launcher.Launcher.mainWithExitCode(Launcher.java:415)
            at org.codehaus.plexus.classworlds.launcher.Launcher.main(Launcher.java:356)
    Caused by: java.lang.NullPointerException
            at org.apache.maven.DefaultMaven.doExecute(DefaultMaven.java:270)
            at org.apache.maven.DefaultMaven.execute(DefaultMaven.java:155)
            ... 11 more
    [ERROR] 
    [ERROR] To see the full stack trace of the errors, re-run Maven with the -e switch.
    [ERROR] Re-run Maven using the -X switch to enable full debug logging.
    [ERROR] 
    [ERROR] For more information about the errors and possible solutions, please read the following articles:
    [ERROR] [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/InternalErrorException
