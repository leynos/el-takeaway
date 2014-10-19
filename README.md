# El Takeaway

A tool to manage data retrieved from the Ello social network

## Usage

chmod 500 the `et` binary and place it somewhere in your executable path.

`et command [options ...]`

Where command is one of:

pull - retrieve the latest published articles from a given user:

`et pull username`

Specify a username to retrieve posts from.
Subsequently, this username may be omitted.

This is intended to be used in conjunction with a version control tool such as git or mercurial to allow you to more easily track the changes you have made to your Ello posts and comments.

## Limitations

Your profile needs to be public.  I should be fixing this shortly, but in the meantime, you can extract the Ello cookie from your Firefox profile (assuming you use Firefox) and supply this to the curl command in the script.

## Prerequisites

This tool was developed on FreeBSD, but I don't see any reason why it shouldn't run on Linux or Mac OS X.  It uses bash, curl, grep, awk and jq.  The latter is the only component that may not be installed on your system by default.  Consult your operating system handbook for instructions on installing this.  Just kidding.  The instructions are [here](https://stedolan.github.io/jq/download/).

## Disclaimers etc.

This software is provided "AS IS" in the hope that someone may find it useful.  If it deletes all your backed up Ello posts, please don't kill me.

Ello is probably a trademark of Modeset or Paul Budnitz or someone.  Its usage here is not intended to imply any endorsement, association or any other kind of relationship or representation.
