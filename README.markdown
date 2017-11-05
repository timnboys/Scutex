# Scutex

Scutex, pronounced (sec-u-techs), is a 100% managed .Net Framework licensing platform for your applications. Scutex is a flexible licensing system providing multiple licensing schemes allowing you the most control over how you license your products. Unlike any other licensing system on the market, Scutex provides 4 distinct licensing schemes, allowing you to protect your products at different levels using completely different licensing schemes, key types and protection systems.

Using Scutex you can create trial versions of your software products and allow your users to buy and use license keys or keyfiles to unlock your product. You can also have edition based licensing to unlock only select features based on the level of the license. Scutex supports upgrade licenses as well as allowing your customers who have an existing version of your product to upgrade to a new version.

This fork is trying to continue to build upon where wavetech left off(and hopefully make it into the full potentional this licensing system has)

## Features

	* Multiple License Keys
	* Backend Service
	* Multi Use Keys
	* Offline Keys
	* Hardware Locking (Online and Offline)
	* Edition Management
	* Upgrade Keys

## License

This software will be licensed by our License included with Weather4U(one of our other software)


## Infragistics Components

~~As of the 10/30/2011 checkin the Infragistics dependancy has been removed.~~
Infragistics is irrevelant at this point since it isn't even used anymore.

## Official Builds & Releases

Will be released here or our website http://keyedinsoftware.org

## Prerequisites

You will need the .Net Framework 4 and SQL Server or SQL Express to use Scutex. To develop Scutex you will need the following installed.

	* Visual Studio 2017 Or better this will be developed in 2017 starting since 11/4/17 (WPF/MSTest)
	* ~~SQL Server 2005/2008/2008 R2 or SQL Express 2005/2008 R2~~ recommended latest MS SQL Server Version Available
	* ~~Microsoft MOLES & Pex Power Tools <http://research.microsoft.com/en-us/projects/pex/>~~ Replaced by Intellitest since Pex/Moles was superceded by Intellitest according to Microsoft.
	* IIS, IIS Express or Casini for testing Services

## Unit Testing

I moved the unit tests from NUnit to MSTest to get integrated MOLES support, and to play around with Pex a little. Unfortunately the way MSTest plays and moves things around it makes getting the paths for required files a major issue. The ReSharper Unit Test Runner does not have that issue, and still runes the MOLES tests. If you run the unit tests from within Visual Studio using MSTest all the test dependent on location will fail. Additionally the performance of the unit tests went downhill due to how MSTest wires things up. Eventually I'll get back in there are refactor the Setup and Teardowns so that they work with MSTest.

## Supported License Key Types

There are two license key types supported:

    * Small Static License Key (SSK) XXX-XXXXXX-XXXX
	* Large Static License Key (LSK) XXXXX-XXXXX-XXXXX-XXXXX-XXXXX
	
The small static key only supports basic license key functionality, while the large static key supports many licensing scenarios.

