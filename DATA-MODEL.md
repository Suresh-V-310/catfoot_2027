# DATA-MODEL

Entities:
- users(id, name, email, role)
- events(id, name, slug, status, start, end, description, tracks, prizes)
- teams(id, name, members, eventId)
- submissions(id, team, project, track, status, repo, eventId, created)
- judges(id, name, assigned[])
- scores(submissionId, judgeId, innovation, technical, impact, design)
- gallery(submissionId, votes, comments)
- audit(time, actor, action)

Scores use a weighted rubric:
Innovation 25%, Technical 35%, Impact 25%, Design 15%.
The displayed normalized score is the mean of available judge scores.
