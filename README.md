# not-binary-presence
This automation is inspired by exellent blog [Making Home Assistant’s Presence Detection not so Binary](https://philhawthorne.com/making-home-assistants-presence-detection-not-so-binary/) by Phil Hawthorne. The code were slightly simplified and improved. 

# how to use
<p>Create user(s) following this pattern:

```
person.person1
person.person2
```

You can create as many persons as You like.
Next create `input_select` helper with following pattern:

```
input_select.person1
input_select.person2
...
```

for each person. 

Create template sensor for each person and add them to dashboard. Optionaly You can customize them by adding a picture with `customize` section in Home Assistant `configuration.yaml` file. Put the picture file into `www` folder and access it with `/local/profile-pic.jpg`.

Now each sensor will have corresponding person home presence status
