# Publication entry schema

Every entry in `_publications/` uses YAML front matter with the following fields:

- `title` (string, required)
- `venue` (string, required) - the venue where the work appears
- `year` (string, required)
- `status` (string, required) - `Published`, `Accepted` or `Under Review`
- `course` (string, required) - course code of the seminar that owns the paper
- `authors` (list of strings, required)
- `codeurl` (string, optional) - canonical URL of the released code. Only record
  this when the paper's code has actually been released and is usable. Do not
  record placeholder, pre-release or mirror repositories. Code that lives in a
  dedicated repository is linked as `https://github.com/<account>/<repo>`; code
  that lives in the shared lab code archive is linked as
  `https://github.com/<account>/<archive-repo>/tree/main/<subdir>`.
- `release_lead` (string, optional) - the person who owns the code release.

## Release-lead policy

By default, the release lead for a paper is the instructor of the course named in
its `course` field. If the program office or a course announcement explicitly
announces a different release lead for a particular paper, that person takes
precedence for that paper only.
