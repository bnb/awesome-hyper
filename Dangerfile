# Ensure there is a summary for a pull request
#fail 'Please provide a summary in the Pull Request description' if github.pr_body.length < 5

# Warn if pull request is not updated
#warn 'Please update the Pull Request title' if github.pr_title.include? 'Update README.md'

# Verifies capitalization of HyperTerm

diff = git.diff_for_file['README.md']
fail 'Please use the approved capitalization for HyperTerm' if diff && diff.patch =~ 'Hyperterm'
