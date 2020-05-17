# Osmosis

[![](https://jitpack.io/v/moe.sunjiao/osmosis.svg)](https://jitpack.io/#moe.sunjiao/osmosis)

My own branch of Osmosis.

Unlike a disgusting official version, you can use XmlReader with an InputStream in my Osmosis.

My XmlReader works in same way as the PbfReader.
If PbfReader can use an InputStream, I don't understand why XmlReader cannot do the same thing.

If someone is biased against me, or feels that my commits will stain their repository, I would rather maintain a version myself.

Related Pull-request:

https://github.com/openstreetmap/osmosis/pull/64

# Use

Add following maven repository in your root build.gradle file:

```
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```

Add the dependency to your module-level build.gradle file (choose the required subproject according to your needs):

```
dependencies {
    implementation 'moe.sunjiao.osmosis:osmosis-apidb:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-areafilter:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-core:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-dataset:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-extract:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-hstore-jdbc:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-osm-binary:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-pbf:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-pbf2:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-pgsimple:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-pgsnapshot:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-replication:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-replication-http:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-set:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-tagfilter:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-tagtransform:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-testutil:0.48.0'
    implementation 'moe.sunjiao.osmosis:osmosis-xml:0.48.0'
}
```
