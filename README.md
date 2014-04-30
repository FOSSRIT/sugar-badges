sugar-badges
============

Sugar Badges Library

This library is used to add a badge feature to your Sugar activity or game.  Badges can be used to reward users who have met certain requirements decided by you!

Badges can be displayed by installing and running the Sash activity found here https://github.com/FOSSRIT/Sash

sugar-badges is pip installable (using the command "pip install sugar-badges"). We recommend doing your development with sugar-badges in a virtual environment just to be safe.

To use the badge library in your existing project you will need to add this line to the top of your Python file:

```python
    from sugar_badges import badges
```

To enable badges in your game, add this line to your init:

```python
    self.badges = badges(activity_name, activity_bundle_id)
```

And finally, to award badges you should make a call to the award method in badges.py using this format:

```python
    self.badges.award(badge_name, badge_description)
```

Badge images should be stored in a badges folder. The filenames should match the badge names you use when calling "award".

To see an example of an activity that has badges already added to it, check out the code for the SkyTime game https://github.com/FOSSRIT/SkyTime
