## Russhian Roulette

`node main.js` for a 1/6 chance of posting your SSH private key on pastebin :)

### Known issues

The actual probability of this software publishing a user's SSH private key is often closer to 0/6, lower than the intended 1/6. In particular, this reduction in functionality will be observed by most users of recently generated SSH key pairs. At the time that Russhian Roulette was designed and developed, ssh-keygen generated RSA key pairs by default. With budget constraints in mind, the decision was made to limit the scope of the implementation to environments for which the assumption holds that keys were generated with the default ssh-keygen behaviour. The default behaviour of ssh-keygen has drifted over time, towards no longer generating RSA key pairs by default. This has led to many more Russhian Roulette users than could be anticipated running the application in environments where it is unable to locate the SSH private key file. The Russhian Roulette team recognises that such a loss of utility is regrettable, and is investigating the feasibility of editing like literally one single string in the source code.
