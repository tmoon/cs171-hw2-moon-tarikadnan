1. Calendar:

    - udience: contributors, visitors, project managers;
    - Data:
        a. pull requests
        b. issues opened
        c. commits
    - Many Pushes: If this happens, then the single date will become the darkest color on the scale. To ensure that a clear gradient is established, the scale itself could dynamically scale based on the total number of degrees of magnitude.

2. Contributors:

    Audience: contributors, project managers;
    Data:
        contributors: /repos/:owner/:repo/events, then go through the JSON file and find all of the individuals who have made commits.
        number of pushes to master per date: /repos/:owner/:repo/events.
        lines added/removed per push: /repos/:owner/:repo/commits, then /repos/:owner/:repo/commits/:sha for each commit. In stats, get additions and deletions.
    Many Pushes: If this happens, then the scale of the graph will change. One could simply increase the size of each user's display window in the screen to ensure the most frequent contributors are still able to show some commits in their chart.

3. Commit Activity:

    Audience: contributors, project managers (mostly the latter);
    Data:
        commits per date: /repos/:owner/:repo/commits, and for each, get date.
    Many Pushes: This would throw off the scale of the bar graph - to fix this, the bar graph would have to be dynamic between weeks in the week view.

4. Code Frequency:

    Audience: contributors, project managers (mostly the former);
    Data:
        additions/deletions per date /repos/:owner/:repo/commits, then /repos/:owner/:repo/commits/:sha for each commit. In stats, get additions and deletions.
    Many Pushes: This would potentially alter the scale of the graph, however if the pushes are that frequent, each would probably not contain a great deal of changes, therefore it would not likely present a huge problem.
5. Punchcard:

    Audience: project managers;
    Data:
        Number of commits per date: commits per date: /repos/:owner/:repo/commits, get all for each date.
        Time of commit: parse out the time from above.
    Many Pushes: This could present a problem of the scale of the circles - to adjust this, perhaps adding layered circles would help, e.g. using red for the first 10, orange for the next 10, etc., layered on top of each other.

6. Pulse:

    Audience: contributors, project managers;
    Data:
        proposed pull requests: /repos/:owner/:repo/pulls, get created_at for date.
        merge requests
        active & new issues: /issues, get created_at, as well as closed_at.
        commits: /repos/:owner/:repo/commits, get all for each date.
        branches
        authors
        additions/deletions: /repos/:owner/:repo/commits, then /repos/:owner/:repo/commits/:sha for each commit. In stats, get additions and deletions.
        files
        commit comments: /repos/:owner/:repo/comments, as well as each created_at.
    Many Pushes:


GitHub Network Graph:
1. Here it seems that 

1. Role of interaction: slide, show what is commited
2. 