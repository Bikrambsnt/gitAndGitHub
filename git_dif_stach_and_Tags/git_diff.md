
# Git diff

Git diff is the informational cmd to check the difference between 2 files or any comparison of two things.

### cmd

git diff 
<!-- here we have to tell which two comarision I want -->


git diff --staged [Stages is the area created after git add]

<!-- Output

diff --git a/git_dif_stach_and_Tags/diff.txt b/git_dif_stach_and_Tags/diff.txt
new file mode 100644
index 0000000..8745996
--- /dev/null
+++ b/git_dif_stach_and_Tags/diff.txt
@@ -0,0 +1,3 @@
+
+Contains some Information.
+
:

 -->

now it gaves me the information of that file..

in this there is a sign of ++ and --
that doesnt means that the file is removed or added

++ and -- refers to the context of two different files

++ refer to one file context and
-- refer to another file context..

#### More cmd

  we can diff branches also 

  git diff <branch1>..<branch2>  [..should be placed between two branch]
  example git diff master..python

  comparing specific commits

  git diff <commit-hash-one> <commit-hash-two>
  example git diff 4b81733..60a0a1b