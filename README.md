# Mesos Utils

Scala utilities for building distributed systems on top of Mesos.

## Usage

We cut releases for each recent Mesos version. Current releases are:

* Mesos `0.16.0` - mesos-utils `0.16.0-1`
* Mesos `0.17.0` - mesos-utils `0.17.0-1`
* Mesos `0.18.0` - mesos-utils `0.18.0-1`

### Maven

Add the Mesosphere repository and the dependency to your `pom.xml`:

    <properties>
        <mesos-utils.version>0.18.0-1</mesos-utils.version>
    </properties>
    ...
    <repositories>
        <repository>
            <id>mesosphere-repo</id>
            <name>Mesosphere Repo</name>
            <url>http://downloads.mesosphere.io/maven</url>
        </repository>
    </repositories>
    ...
    <dependencies>
        <dependency>
            <groupId>mesosphere</groupId>
            <artifactId>mesos-utils</artifactId>
            <version>${mesos-utils.version}</version>
        </dependency>
    </dependencies>

### SBT

Add this to your SBT config:

    resolvers += "Mesosphere Repo" at "http://downloads.mesosphere.io/maven"
    libraryDependencies += "mesosphere" % "mesos-utils" % "0.18.0-1"
