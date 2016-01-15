# IRC Operator information

## Links 

- [Snoonet channel modes](https://snoonet.org/modes)
- [Snoonet user modes](https://snoonet.org/umodes)

See also `/msg ChanServ help [command]` with `[command]`

- `AOP` set a collection of access flags giving high level of access.
- `ACCESS` set access in a medium-grained way via a numeric level.
- `FLAGS` set access in a fine-grained with via lettered flags.


## Channel Access

Setting/seeing who has what permission over the channel settings.

Give ultimate access to exactly one individual:

```
/msg ChanServ SET FOUNDER #CHANNEL *!*@HOSTNAME
```

Give full access:

```
/msg ChanServ AOP #CHANNEL ADD *!*@HOSTNAME
```

List full access

```
/msg ChanServ AOP #CHANNEL LIST
```

More fine grained via ACCESS

```
/msg ChanServ ACCESS #CHANNEL LIST
/msg ChanServ ACCESS #CHANNEL VIEW
```


## Channel info

See all modes:

```
/mode #CHANNEL
```

## Private Channels

Make channel invite-only, private and secret

```
/mode #CHANNEL +ips
```

Allow anyone to invite others:

```
/mode #CHANNEL +A
```

Invite someone once:

```
/invite NICK
```

Make the invite permanent:

```
/mode #CHANNEL +I *!*@HOSTNAME
```
