1. Phar extension required

2. Ensure that the. / tar / tar.proto.php file under the project exists and contains the following contents

` ` ` `

return array(

'appName' = >

'servername' = >

...

);

` ` ` `

3. Introduce tar deploy to composer.json of the project.

4. Add the following content to the project composer.json:

` ` ` `

"Scripts": {

"deploy": "\\Tars\\deploy\\Deploy::run"

}

` ` ` `

5. Execute the following command in the project directory to generate the project compression package to be uploaded.
```
    composer run-script deploy
```