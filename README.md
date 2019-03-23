# NAME

Mojolicious::Plugin::NoServerHeader - Removes the Server header from every Mojolicious response

# SYNOPSIS

    # Mojolicious::Lite
    plugin 'NoServerHeader';

    # Mojolicious
    $app->plugin('NoServerHeader');

# DESCRIPTION

[Mojolicious::Plugin::NoServerHeader](https://metacpan.org/pod/Mojolicious::Plugin::NoServerHeader) removes the default Server header, "Mojolicious (Perl)", from every response.
This can be useful for security reasons if there was ever a known exploit for [Mojolicious](https://metacpan.org/pod/Mojolicious). If you are really concerned about
this, you should also change the default error pages like the [failraptor](https://mojolicious.org/mojo/failraptor.png), although
those are probably less obvious than a Server header in every response.

# AUTHOR

Adam Hopkins <srchulo@cpan.org>

# COPYRIGHT

Copyright 2019- Adam Hopkins

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl it.

# SEE ALSO
