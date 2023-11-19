# change-root-password

Role for change root password and sett i attr in `/etc/shadow` file.

## Deploy example

```yaml
  roles:
    - role: change-root-password
      root_password: "{{ something | password_hash('sha512') }}"
```

## Available parameters

### Main

| Param | Default | Description |
| -------- | -------- | -------- |
| `root_password` | `-` | Root password in sha512. |
