A play-by-email / play-by-web moderator for the boardgame Terra Mystica.

- Full rules enforcement, automatic email notifications, command language + simple UI
- Written in Perl and JavaScript
- Uses PostgreSQL as the backing storage


# Deployment Instructions

## make logs directories

```bash
mkdir logs
mkdir www-devel
mkdir www-devel/logs
mkdir www-devel/data/log
```

```bash
mkdir www-devel
perl deploy.pl www-devel
```


# Perl CPAN modules to install

```
cpanm Bytes::Random::Secure CGI::PSGI Clone Crypt::Blowfish Crypt::CBC Crypt::Eksblowfish::Bcrypt Data::Password::Common DBD::Pg DBI Digest::SHA1 Exporter::Easy File::Slurp indirect JSON Math::Random::MT Method::Signatures::Simple Moose Readonly Statistics::Descriptive Task::Plack Term::ReadLine Text::Diff Text::Template
```

More deployment instructions: https://github.com/jsnell/terra-mystica/wiki/Local-environment-setup
