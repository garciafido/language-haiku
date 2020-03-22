Update the version number in your package's package.json.
The version number must match the regular expression: ^\d+\.\d+\.\d+
Commit the version number change

Create a Git tag referencing the above commit.
The tag must match the regular expression ^v\d+\.\d+\.\d+ and the part after the v must match the full text of the version number in the package.json

Execute git push --follow-tags
Execute apm publish --tag tagname where tagname must match the name of the tag created in the above step

Examples:

    apm publish --tag v1.0.0
    apm unpublish language-haiku@1.0.0

Or:
    apm publish minor
    
--------------------------------------------------------
Remove atom
rm -rf ~/.atom ~/Library/Preferences/com.github.atom.helper.plist ~/Library/Preferences/com.github.atom.plist /Applications/Atom.app /Applications/Atom\ Beta.app /usr/local/bin/atom /usr/local/bin/atom-beta /usr/local/bin/apm /usr/local/bin/apm-beta ~/Library/Application\ Support/Atom/ ~/Library/Application\ Support/com.github.atom.ShipIt ~/Library/Saved\ Application\ State/com.github.atom.savedState ~/Library/Caches/com.github.atom.ShipIt/ ~/Library/Caches/com.github.atom ~/Library/Caches/Atom
-------------------------------------------------------
brew cask install atom
nano /Applications/Atom.app/Contents/Resources/app/apm/bin/python-interceptor.sh


    exec python "${ARGS[@]}"
    ;;
  *)
    exec python "$@"
    ;;

====>

    exec python2 "${ARGS[@]}"
    ;;
  *)
    exec python2 "$@"
    ;;
