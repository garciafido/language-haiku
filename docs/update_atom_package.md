Update the version number in your package's package.json.
The version number must match the regular expression: ^\d+\.\d+\.\d+
Commit the version number change

Create a Git tag referencing the above commit.
The tag must match the regular expression ^v\d+\.\d+\.\d+ and the part after the v must match the full text of the version number in the package.json

Execute git push --follow-tags
Execute apm publish --tag tagname where tagname must match the name of the tag created in the above step

Example:

    apm publish --tag v1.0.0
