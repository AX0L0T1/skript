# Skript #

##Blacklisted Drops##

### Requires: ###
- Skript 2.6.0
- SKBee 1.15.0
- SKRayFall 1.9.26

[Download {185 bytes}](https://docs.google.com/download?test)
```
variables:
	{blacklisted.drops} = 0

every tick:
	{blacklisted.drops} is 0:
		add diamond sword to {blacklisted.drops}

on drop:
	item is in {blacklisted.drops}:
		cancel event
```
