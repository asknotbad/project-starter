# Project starter

Project starter.

## System requirements

TODO: write System requirements

## Ennvironment variables

- DOCKER_NAME — project name for Docker-Compose
- WEB_HOST — <code>localhost</code> for dev or <code>your-domain.com</code> for production
- WEB_PORT — local posrt for web-service (<code>5173</code> or whatever you want)
- TRAEFIK_HOST <code>traefik.localhost</code> for dev or <code>traefik.your-domain.com</code> for production
- TRAEFIK_USER — username for traefik dashboard
- TRAEFIK_PASSWORD — password for traefik dashboard
- LE_ACME_EMAIL — email fo Let'sEncrypt notifications


## Services

### web-service

TODO: write about web-service

### traefik-service

TODO: write about traefik-service

## Development

Copy <code>.env.example</code> into <code>.env</code> and fill all values.

Start project in dev-mode:

```bash
npm run dev
# or
npm run start:dev
```

Go to [localhost](http://localhost) in browser.

Stop project in dev-mode:

```bash
npm run stop:dev
```

## Use in production

Configure your domain DNS-records:

```
A-record your-domain.com = your.server.ip.address
A-record traefik.your-domain.com = your.server.ip.address
```

Copy <code>.env.example</code> into <code>.env</code> and fill all values.

Start project in production-mode:

```bash
npm start
```

Go to [your domain address](http://ypur-domain.com) in browser.

Stop project in production-mode:

```bash
npm stop
```


## Support

[Bugs](https://github.com/asknotbad/project-starter/issues)

## Stay in touch

- Author: [Den Kochetkov](https://github.com/dkochetkov)
- E-mail: <d@asknotbad.com>
- Website: [asknotbad.com](https://asknotbad.com/)

## License

[Apache-2.0](LICENSE)

Copyright &copy; 2025 Not Bad
