# National Anthem Project

A team project from the Git & GitHub Practice Workshop. Three members worked together in one repository to build a small website that displays the Indian National Anthem, "Jana Gana Mana".

## Live Demo

The finished application is running on AWS EC2:
http://16.171.150.234:5000

## Meet the Team

| Member | Role | Main work |
| --- | --- | --- |
| Gagan | Team Lead | Created the repository, merged the branches, resolved the merge conflict, recovered the deleted commit |
| Member 2 | Developer | Built the Flask application, added the first stanza and the English title branch |
| Member 3 | Tester | Added the second line of the stanza and the bilingual title branch, checked the final page |

## The Journey - What Each Part Taught Us

1. **Part 0 - Identities:** Each member set up a separate Git name and email, so every commit shows who did the work.
2. **Part 1 - Publish:** The repository was created on the EC2 instance and published to GitHub.
3. **Part 2 - Push and Pull:** Members shared their work through push and pull instead of sending files to each other.
4. **Part 3 - Branch and Merge:** A separate branch carried the second stanza (two commits), then it was merged into main and deleted.
5. **Part 4 - The Conflict:** Two branches changed the same title line from the same starting commit. Merging created a conflict, and it was resolved by keeping the bilingual title: "Bharat ka Rashtragan - Jana Gana Mana".
6. **Part 5 - Recovery:** A commit was deleted using git reset and then brought back using git reflog.

## Repository at a Glance

| Fact | Detail |
| --- | --- |
| Total commits | 11 |
| Contributors | 3 |
| Branches today | Only main (all work branches merged and deleted) |
| Final page title | Bharat ka Rashtragan - Jana Gana Mana |
| Workshop status | All six checkpoints passed |

## Project Files

```
anthem-workshop/
|-- anthem.txt          (the anthem text)
|-- app.py              (the Flask application)
|-- requirements.txt    (Python packages needed)
|-- .gitignore
|-- README.md
|-- templates/
    |-- index.html      (the web page)
```

## Run It Yourself

```
git clone https://github.com/foraws832-dotcom/anthem-workshop.git
cd anthem-workshop
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python3 app.py
```

Then open http://localhost:5000 in a browser.

## Four Things We Take Away

- A branch is only a small pointer to a commit. Creating one copies nothing.
- Always pull before starting work, and push when the work is done.
- A merge conflict is not an error - it is Git asking a person to decide.
- Committed work can be recovered with git reflog. Uncommitted work cannot.

## Repository Link

https://github.com/foraws832-dotcom/anthem-workshop
