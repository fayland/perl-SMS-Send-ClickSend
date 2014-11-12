[![Build Status](https://travis-ci.org/fayland/perl-SMS-Send-ClickSend.svg?branch=master)](https://travis-ci.org/fayland/perl-SMS-Send-ClickSend)
[![Coverage Status](https://coveralls.io/repos/fayland/perl-SMS-Send-ClickSend/badge.png?branch=master)](https://coveralls.io/r/fayland/perl-SMS-Send-ClickSend?branch=master)
[![Gitter chat](https://badges.gitter.im/fayland/perl-SMS-Send-ClickSend.png)](https://gitter.im/fayland/perl-SMS-Send-ClickSend)

# NAME

SMS::Send::ClickSend - SMS::Send joins SMS::ClickSend

# SYNOPSIS

    use SMS::Send;

    my $sender = SMS::Send->new('ClickSend',
        _username => 'username',
        _api_key => 'api_key',
    );

    # Send a message
    my $sent = $sender->send_sms(
        text => 'This is a test message',
        to   => '+61411111111',
    );

    # Did the send succeed.
    if ( $sent ) {
        print "Message sent ok\n";
    } else {
        print "Failed to send message\n";
    }

# DESCRIPTION

Please read [SMS::ClickSend](https://metacpan.org/pod/SMS::ClickSend) for more details.

# send\_sms

that's wrap of **send** on [SMS::ClickSend](https://metacpan.org/pod/SMS::ClickSend)

# AUTHOR

Fayland Lam <fayland@gmail.com>

# COPYRIGHT

Copyright 2014- Fayland Lam

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO
