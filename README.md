# kernelrepo
docs: kbuild: convert docs to ReST and rename to *.rst

The kbuild documentation clearly shows that the documents
there are written at different times: some use markdown,
some use their own peculiar logic to split sections.

Convert everything to ReST without affecting too much
the author's style and avoiding adding uneeded markups.

The conversion is actually:
  - add blank lines and identation in order to identify paragraphs;
  - fix tables markups;
  - add some lists markups;
  - mark literal blocks;
  - adjust title markups.

At its new index.rst, let's add a :orphan: while this is not linked to
the main index.rst file, in order to avoid build warnings.

Signed-off-by: Mauro Carvalho Chehab <mchehab+samsung@kernel.org>
Signed-off-by: Jonathan Corbet <corbet@lwn.net>
