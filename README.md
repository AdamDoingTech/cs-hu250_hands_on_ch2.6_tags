# Ch2.6
# Exercise: Investigating Tags

## Step 1
Familiarize yourself with the repository by checking the repository history, file structure, file contents, etc.

## Step 2
Use the following command to display the list of tags contained in this repository:
```bash
$ git tag
```

## Step 3
Use the following command to display the history of commits annotated with the location of the tags (i.e., it shows which commit a tag is pointing to):
```bash
$ git log --oneline --decorate
```

## Step 4
Use the following command to show the details of the last commit:
```bash
$ git show
or
$ git show HEAD
or
$ git show HEAD~0
```

Since the last commit is tagged with an annotated tag (called `v1.0`), you can use the following command to show the details of the annotated tag, as well as the details of the commit.
```bash
$ git show v1.0
```

## Step 5
Use the following command to show the details of the antepenultimate (i.e., the third most recent) commit:
```bash
$ git show HEAD~2
or
$ git show <abbreviated_sha_of_antepenultimate_commit>
```

Since the antepenultimate commit is tagged with a lightweight tag (called `v1.0-beta`), the following command will display only the details of the commit, since the lightweight tag has no additional details.
```bash
$ git show v1.0-beta
```

## Step 6
Run the `./chaos_monkey.sh` script.

## Step 7
Use the command from `Step 3` to investigate the new changes made to the repository by the `./chaos_monkey.sh` script.

## Step 8
List all the tags that are currently in the repository.
