# git audit

## Git commits to commit

1.  Did the student navigate to the <code>work</code> directory and create a subdirectory named <code>hello</code> ?
    ![sub dir](scrImg/250317_01GitInit.jpg)

2.  Did the student generate a file named <code>hello.sh</code> with the content **echo "Hello, World"** inside the <code>hello</code> directory?
3.  Did the student initialize a Git repository in the <code>hello</code> directory?
4.  Did the student use the <code>git status</code> command to check the status of the repository?
    ![git status](scrImg/250317_02GitStatus.jpg)
5.  Did the student modify the <code>hello.sh</code> file content with the provided **echo "Hello, $1"** ?
    ![2nd commit](scrImg/250317_04Git-SecondCommit.jpg)
6.  Did the student stage the modified <code>hello.sh</code> file, commit the changes to the repository, and ensure that the working tree is clean afterward?
7.  Did the student further modify the <code>hello.sh</code> file to include comments, and then make two separate commits as instructed?
8.  Did the student make two separate commits, with the first commit for the comment in **line 1** and the second commit for the changes made to **lines 3 and 4** , as instructed?
    ![git log](scrImg/250317_06Git-Log.jpg)

## History

9.  Did the student display the Git history of the working directory with the <code>git log</code> command? See image above
10. Did the student successfully display a condensed view of the Git history, showing only commit hashes and messages using the "One-Line History" format?
    
    ![one-line](scrImg/250317_07Git-Log-Oneline.jpg)
11. Was the student able to customize the log output to display the last 2 entries?
    ![last 2](scrImg/250317_08Git-Log-Last2Items.jpg)
12. Did the student successfully demonstrate viewing commits made within the last 5 minutes?
    ![last 5min](scrImg/250317_09Git-Log-Last5Mins.jpg)
13. Did the student successfully customize the format of Git logs and display them according to this example \* e4e3645 2023-06-10 | Added a comment (HEAD -> main) [John Doe]?
    ![custom log](scrImg/250317_10Git-Log-Personalize.jpg)

## Check it out

14. Did the student successfully restore the first snapshot of the working tree and print the content of <code>hello.sh</code> ?
    ![restore 1st](scrImg/250317_11Git-Checkout-1stSnapshot.jpg)
15. Did the student successfully restore the second recent snapshot and print the content of <code>hello.sh</code> ?
    ![restore 2nd](scrImg/250317_12Git-Checkout-2ndCommit.jpg)
16. Did the student ensure that the working directory reflects the latest version of <code>hello.sh</code> from the main branch without using commit hashes?

    ![latest main branch](scrImg/250317_14Git-Checkout-Back-to-Latest.jpg)

## TAG me

17. Did the student successfully tag the current version of the repository as **v1** ?
    ![tag v1](scrImg/250317_15Git-Tag-Latest-v1.jpg)
18. Did the student successfully tag the version immediately prior to the current version as **v1-beta** , without relying on commit hashes?
    ![tag v1-beta](scrImg/250317_16Git-Tag-Previous-v1-beta.jpg)
19. Did the student navigate back and forth between the two tagged versions, **v1** and **v1-beta** ?
20. Did the student display a list of all tags present in the repository to verify successful tagging?
    ![all tags](scrImg/250317_17Git-Tag-all-tags.jpg)

## Changed your mind?

21. Did the student successfully revert the modifications made to the latest version of the file, restoring it to its original state before staging using a **Git** command?
    ![latest version](scrImg/250317_18Git-ChangeMe-latest.jpg)
22. Did the student introduce unwanted changes to the file, stage them, and then successfully clean the staging area to discard the changes?
    ![unwanted changes](scrImg/250317_19Git-ChangeMe-BadComment.jpg)
23. Did the student add unwanted changes again, stage the file, commit the changes, and then revert them back to their original state?
    ![original state](scrImg/250317_20Git-ChangeMe-Revert-to-default-comment.jpg)
    ![revert back](scrImg/250317_22Git-Revert-reverted-back-to-original.jpg)
24. Did the student tag the latest commit with oops and remove commits made after the v1 version, ensuring that the HEAD points to v1?
    ![oops](scrImg/250317_24Git-Tag-oops.jpg)
25. Did the student display the logs with the deleted commits, particularly focusing on the commit tagged **oops** ?
    ![tag oops](scrImg/250317_25Git-Tag-Removed-oops.jpg)
26. Did the student ensure that unreferenced commits were deleted from the history, with no logs remaining for these deleted commits?
    ![delete commits](scrImg/250317_26Git-Tag-Show-logs-with-deleted-commits.jpg)
    ![removed delete commits](scrImg/250317_27Git-Tag-removed-deleted-commits.jpg)
27. Did the student add author information to the file and commit the changes?
    ![author](scrImg/250317_28Git-Tag-Author-details-added.jpg)
28. Did the student update the file to include the author email without making a new commit, but included the change in the last commit?
    ![author email](scrImg/250317_29Git-Tag-Author-Email-added.jpg)

## Move it

29. Did the student successfully move the <code>hello.sh</code> program into a <code>lib/</code> directory using Git commands?
    ![mv to lib](scrImg/250317_31Git-Move-moved-hello-to-lib-dir.jpg)
30. Did the student commit the move of <code>hello.sh</code> ? see above image
31. Did the student create and commit a <code>Makefile</code> in the root directory of the repository with the provided content?
    ![Makefile](scrImg/250317_32Git-Move-Makefile-created.jpg)

## blobs, trees and commits

32. Ask the student to navigate to the <code>.git/</code> directory and explain to you the purpose of each subdirectory, including **objects/**, **config**, **refs** , and **HEAD** .
    ![nav git](scrImg/250317_33Git-Move-git-dir.jpg)
33. Was the student able to explain the purpose of each subdirectory, including **objects/** \*/, **config** , **refs** , and **HEAD** ?
    ![explain](scrImg/250317_34Git-Move-Explain-items.jpg)
34. Did the student successfully find the latest object hash within the <code>.git/objects/</code> directory using Git commands?
    ![obj hash](scrImg/250317_35Git-Move-git-objects-hash.jpg)
35. Was the student able to print the type and content of this object using Git commands?
    ![print type](scrImg/250317_36Git-Move-object-type-content.jpg)
36. Did the student use Git commands to dump the directory tree referenced by a specific commit? see image above
37. Were they able to dump the contents of the <code>lib/</code> directory and the <code>hello.sh</code> file using Git commands?
    ![dump](scrImg/250317_37Git-Move-dump-directory-tree.jpg)

## Branching, Merging & Rebasing

38. Did the student successfully create and switch to a new branch named <code>greet</code> ?
    ![greet branch](scrImg/250317_38Git-Branch-greet.jpg)
39. Did the student create and commited a new file named <code>greeter.sh</code> in the <code>lib</code> directory with the provided code in it?
    ![greeter file](scrImg/250317_39Git-Branch-lib-greeter.jpg)
    ![greeter commit](scrImg/250317_40Git-Branch-lib-greeter-commit.jpg)
40. Did the student update the <code>lib/hello.sh</code> file with the provided content, stage, and commit the changes? see above image
41. Did the student update the <code>Makefile</code> with the comment, stage, and commit the changes?
    ![Makefile](scrImg/250317_43Git-Branch-Makefile.jpg)
    ![Makefile update](scrImg/250317_45Git-Branch-Makefile-commit.jpg)
42. Was the student able to compare and show the differences between the <code>main</code> and <code>greet</code> branches for the <code>Makefile</code >, <code>hello.sh</code> , and <code>greeter.sh</code> files?
    
    ![main](scrImg/250317_46Git-Branch-Makefile-main-branch.jpg)
    ![diff1](scrImg/250317_47Git-Branch-Makefile-Compare-diff.jpg)
    ![diff2](scrImg/250317_48Git-Branch-Makefile-Compare-diff2.jpg)
43. Did the student generate a **README.md** file with the provided content and commit it?
    ![Readme](scrImg/250317_49Git-Branch-Readme-file.jpg)
44. Did the student draw a commit tree diagram illustrating the diverging changes between all branches to demonstrate the branch history?
    ![tree](scrImg/250317_52Git-Branch-Tree-Diagram-detailed.jpg)

## Conflicts, merging and rebasing

45. Did the student successfully merge the changes from the <code>main</code> branch into the <code>greet</code> branch?
    ![merge](scrImg/250317_54Git-Conflict-Merge-Rebase-main-into-greet2.jpg)
46. Did the student make the specified changes to the <code>hello.sh</code> file in the <code>main</code> branch and commit them?
    ![commit](scrImg/250317_57Git-Conflict-Merge-Rebase-update-hello-main-branch-commit.jpg)
47. Did the student attempt to merge the <code>main</code> branch into the <code>greet</code> branch creating a conflict during the merge?
    ![conflict](scrImg/250317_58Git-Conflict-Merge-Rebase-merge-main-greet-conflict.jpg)
48. Did the student successfully resolve the conflict, accepting changes from the main branch?
    ![resolve](scrImg/250317_61Git-Conflict-Merge-Rebase-merge-main-greet-conflict-removed2.jpg)
49. Did the student commit the conflict resolution changes?
    ![commit](scrImg/250317_62Git-Conflict-Merge-Rebase-merge-main-greet-conflict-resolved3.jpg)
50. Did the student return to the point before the initial merge between <code>main</code> and <code>greet</code> ? see image above
51. Did the student rebase the <code>greet</code> branch on top of the latest changes in the <code>main</code> branch?
    ![rebase](scrImg/250317_63Git-Conflict-Merge-Rebase-successful.jpg)
52. Did the student successfully merge the changes from the <code>greet</code> branch into the <code>main</code> branch?
    ![merge](scrImg/250317_64Git-Conflict-Merge-Rebase-merge-greet-into-main.jpg)
53. Ask the student to explain the difference between merging and rebasing and if he understand Fast-Forwarding.

### Fast-Forwarding

- Happens when main has no new commits since greet branched off.
- Instead of creating a merge commit, Git just moves main forward to greet's latest commit.
- No extra commit is created.

```bash
Before Merge:
main:  A---B
greet:     \---C---D

After Fast-Forward Merge:
main:  A---B---C---D  (main just moves forward)
```

### Merge

- Happens when main and greet both have new commits.
- Git creates a new merge commit that combines both histories.

```bash
Before Merge:
main:  A---B---E---F
greet:      \---C---D

After Merge:
main:  A---B---E---F---M (Merge Commit)
                \---C---D
```

### Rebase

- Linear rewrites history
- Changes commit hashes
- Clean history, collaboration

```bash
Before Rebase:
main:  A---B---E---F
greet:      \---C---D

After Rebase:
greet:  A---B---E---F---C'---D'
```

54. Did the student demonstrate an understanding of fast-forwarding?
55. was the student able to explain the difference between merging and rebasing?

## Local & Remote Repo

56. Did the student complete the cloning process of the <clone>hello</clone> repository to <clone>cloned_hello</code> ?
    ![cloning](scrImg/250317_66Git-LocalRemotRepo-cloned-hello.jpg)
57. Did the student fetch and merge changes from the remote repository into the <code>main</code> branch?
    ![main](scrImg/250317_67Git-LocalRemotRepo-list-all.jpg)
58. Did the student list both remote and local branches, make changes to the original repository, and synchronize the cloned repository with remote changes?
    ![list branches](scrImg/250317_67Git-LocalRemotRepo-logged.jpg)
59. Did the student successfully clone the <code>hello</code> repository into the <code>work/</code> directory as <code>cloned_hello</code> , without using the copy command? see quest56 image above
60. Did the student show the logs for the <code>cloned_hello</code> repository? see quest58 image above
61. Did the student display the name of the remote repository **(origin)** and provide more information about it?
    ![remote origin](scrImg/250317_68Git-LocalRemotRepo-show-origin.jpg)
62. Did the student list all remote and local branches in the <code>cloned_hello</code> repository?
    ![remote local](scrImg/250317_69Git-LocalRemotRepo-list-remote-local-branches.jpg)
63. Did the student make changes to the original repository, update the **README.md** file with the provided content, and commit the changes?
    ![readme](scrImg/250317_69Git-LocalRemotRepo-original-readme-changed.jpg)
64. Inside the cloned repository <code>cloned_hello</code>, did the student fetch the changes from the remote repository and display the logs, ensuring commits from the <code>hello</code> repository are included?
    ![logs](scrImg/250317_70Git-LocalRemotRepo-fetch-remote-repo-logs.jpg)
65. Did the student merge the changes from the remote <code>main</code> branch into the local <code>main branch?
    ![merge](scrImg/250317_71Git-LocalRemotRepo-merge-remote-main-into-local-main.jpg)
66. Did the student add a local branch named <code>greet</code> tracking the remote <code>origin/greet</code> branch?
    ![origin greet](scrImg/250317_72Git-LocalRemotRepo-local-greet-to-track-remote-greet.jpg)
67. Did the student add a <code>remote</code> reference to their Git repository?
    ![add remote](scrImg/250317_73Git-LocalRemotRepo-remote-add-to-repo.jpg)
68. Did the student push the <code>main</code> and <code>greet</code> branches to the <code>remote</code> repository?
    ![push-main-greet-remote](scrImg/250317_74Git-LocalRemotRepo-push-main-greet-remote-branches.jpg)

### Ask the following question to the student:

**What is the single git command equivalent to what you did before to bring changes from remote to local <code>main</code> branch?**

69. Did the student provide an accurate response?
    <code>git pull --rebase origin main</code>

## Bare Repository

- to create a bare repo <code>git init --bare repo-name.git</code>
- <code>ls repo-name.git</code> the output is

```bash
HEAD
config
description
hooks/
info/
objects/
refs/
```

- Why a bare repo is needed?
  - for collaboration and storage centralization
  - acts as a **remote repo** that many devs can push-to and pull-from
  - GitHub, GitLab, and self hosted Git servers use bare repos
  - prevents accidental changes
  - as there is no **working directory** users cannot modify files directly
  - ensures the central repo remains _clean_
  - useful for deployment and automation
  - CD/CI some workflows use a bare repo with **Git hooks** to deploy code automatically when updates are pushed.

70. Did the student successfully create a bare repository named <code>hello.git</code> from the existing <code>hello</code> repository?
    ![bare repo](scrImg/250317_75Git-BareRepo-create-hello-git.jpg)

71. Did the student add the bare <code>hello.git</code> repository as a remote to the original repository <code>hello<code> ?
    ![add bare hello](scrImg/250317_76Git-BareRepo-add-bare-hello-git.jpg)

72. Did the student change the **README.md** file in the original repository, commit the change, and push it to the shared repository?
    ![readme](scrImg/250317_77Git-BareRepo-change-readme2.jpg)
73. Did the student switch to the cloned repository <code>cloned_hello</code> and successfully pull down the changes just pushed to the shared repository?
    ![switched](scrImg/250317_78Git-BareRepo-switched-cloned-hello.jpg)
    ![pulled changes](scrImg/250317_79Git-BareRepo-pulled-changes.jpg)
    ![updated readme](scrImg/250317_80Git-BareRepo-pulled-changes-readme.jpg)
