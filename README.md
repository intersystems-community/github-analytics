# github-analytics
Repository activities monitoring in DeepSee

## Installation

To install it 
+ Download repository files(eg by cloning)
+ Create namespace(eg GitHubNS)
+ And import all files in crated namespace

## Usage
1.At first launch execute in namespace (that you created for this repository classes, eg GitHubNS) line below

write ##class(GitHub.Task).LoadAll(organizationName, login, password)

Where 
+ organization name takes from organization's github url(eg for [Intersystems corp. Russia](https://github.com/intersystems-ru) organiztionName = "intersystems-ru")
+ login - your login on Github.com
+ password - your password on Github.com
It need login and password for getting data of views and clones of repositories(where you can push) 

2.Every next launch execute next line

write ##class(GitHub.Task).UpdateAll(organizationName, login, password)
