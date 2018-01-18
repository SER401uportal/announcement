# Announcement Portlet to Soffit Conversion

This project is to convert the existing Announcement [Portlet][] by Erik Olsson to the new [Soffit][] set up. 

## Configuration

See also documentation in the [AnnouncementsPortlet wiki on Confluence][].

### Using Encrypted Property Values

You may optionally provide sensitive configuration items -- such as database passwords -- in encrypted format.  Use the [Jasypt CLI Tools][] to encrypt the sensitive value, then include it in a `.properties` file like this:

``` ini
hibernate.connection.password=ENC(9ffpQXJi/EPih9o+Xshm5g==)
```

Specify the encryption key using the `UP_JASYPT_KEY` environment variable.

## Dependencies

These dependencies are expected to be loaded by overall uPortal:

*   [Font Awesome][] 4, last tested with [Font Awesome 4.7.0][]

## Team

*   Ruan Botha
*   Justin Danweber
*   Hannah Do
*   Craig Smith
*   David Worrell

[Portlet]: https://wiki.jasig.org/display/PLT/Jasig+Sponsored+Portlets
[Soffit]: https://github.com/uPortal-Project/soffit-samples
[AnnouncementsPortlet wiki on Confluence]: https://wiki.jasig.org/display/PLT/Announcements+Portlet
[Font Awesome]: http://fontawesome.io/
[Jasypt CLI Tools]: http://www.jasypt.org/cli.html
[Font Awesome 4.7.0]: https://github.com/FortAwesome/Font-Awesome/releases/tag/v4.7.0
