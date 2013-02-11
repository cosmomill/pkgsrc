Getting the "source"
--------------------

#####Downloading a snapshot

The easiest way probably is to download a snapshot. Just select the newest one from the repository and extract it in /usr/pkgsrc:

<pre>
cd ~
wget -O pkgsrc-wip.tar.gz https://github.com/cosmomill/pkgsrc/tarball/master
tar -C /usr/pkgsrc -xvf pkgsrc-wip.tar.gz --strip 1
</pre>

Trying packages
--------------------

Change to the package's directory:

<pre>
cd /usr/pkgsrc/wip/<packagename>
</pre>

Take a look at the TODO file there. If the package seems finished enough, install, and try it out:

<pre>
make install
</pre>

#####Note

If using bootstrap or pkgsrc on a non-NetBSD system, use the pkgsrc bmake command instead of "make" in the examples in this guide.
