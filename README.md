Sublime PHPUnit
===============

This plugin adds PHPUnit support to Sublime Text 2.

Installation
------------

 1. Clone this repository into your packages directory (Sublime Text 2 -> Preferences -> Browse Packages).
 2. If PHPUnit can't be found, add "path_to_phpunit" to your PHPUnit config (Sublime Text 2 -> Package Settings -> PHPUnit -> Settings - User)

PHPUnit Support For Sublime Text 2
----------------------------------

This plugin adds support for running PHPUnit tests from inside Sublime Text 2.

Right-click in the editor to:

* Run all unit tests
* Run the unit tests for the current file
* Run the unit tests in the current file
* Run PHPUnit, using the current XML config file
* Goto the file containing the tests or the file being tested

Right-click in the side-bar to:

* Run the unit tests in the current file
* Run all the unit tests
* Run PHPUnit, using the selected XML config file

You can also open up the Command Palette (CTRL + SHIFT + P on Linux), and type
'PHPUnit' to see what you can do with PHPUnit in the currently open file.

To make this work, you need to create a phpunit.xml.dist or phpunit.xml file for your code (projects using [Phix](http://phix-project.org) get this for free).  The Sublime-PHP plugin searches the folders upwards from whatever you are trying to test, using the first phpunit.xml or phpunit.xml.dist that it finds.  Make sure that your phpunit.xml file is either at the top of your tests folder (or even further up), and this plugin will work for you.

_PHPUnit support is based on the [Ruby Tests plugin](https://github.com/maltize/sublime-text-2-ruby-tests)_

Snippets
--------

We add the following snippets to speed up writing PHP test code.

To use any of the snippets, simply type the name of the snippet, then press the <TAB> key.  Sublime Text 2 will insert the snippet, and you can then use the <TAB> key to move through any placeholders that you need to replace.

- **phpunit-test**: create a new test method inside your TestCase class
- **phpunit-testcase**: create a new TestCase class to put your tests inside
- **assahk**: `assertArrayHasKey()`
- **assae**: `assertAttributeEquals()`
- **asscha**: `assertClassHasAttribute()`
- **asschsa**: `assertClassHasStaticAttribute()`
- **assc**: `assertContains()`
- **assco**: `assertContainsOnly()`
- **asscu**: `assertCount()`
- **asse**: `assertEquals()`
- **assem**: `assertEmpty()`
- **assexml**: `assertEqualXMLStructure()`
- **assf**: `assertFalse()`
- **assfe**: `assertFileEquals()`
- **assfx**: `assertFileExists()`
- **assgt**: `assertGreatherThan()`
- **assgte**: `assertGreaterThanOrEqual()`
- **assio**: `assertInstanceOf()`
- **assit**: `assertInternalType()`
- **asslt**: `assertLessThan()`
- **asslte**: `assertLessThanOrEqual()`
- **assnn**: `assertNotNull()`
- **assn**: `assertNull()`
- **assoha**: `assertObjectHasAttribute()`
- **assre**: `assertRegExp()`
- **asss**: `assertSame()`
- **asssc**: `assertSelectCount()`
- **assse**: `assertSelectEquals()`
- **asssef**: `assertStringEqualsFile()`
- **asssew**: `assertStringEndsWith()`
- **asssmf**: `assertStringMatchesFormat()`
- **asssmff**: `assertStringMatchesFormatFile()`
- **asssre**: `assertSelectRegExp()`
- **assssw**: `assertStringStartsWith()`
- **asst**: `assertTrue()`
- **assta**: `assertTag()`
- **assxmlfef**: `assertXmlFileEqualsXmlFile()`
- **assxmlsef**: `assertXmlStringEqualsXmlFile()`
- **assxmlses**: `assertXmlStringEqualsXmlString()`

Contributions Welcome
---------------------

Requests for features, and pull requests with patches, are most welcome :)
