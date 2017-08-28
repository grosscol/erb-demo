---
layout: slide
title: Examples
---

<section markdown="1">

## Examples

Slides can be nested inside of other slides,  

[![Down arrow](https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png)](#){: .image .navigate-down}

</section>
<section markdown="1">

## Web Frameworks
- Rails
- Sinatra

```html
<h1><%= @greeting %></h1>
<h2><%= @user.name %></h2>
```

</section>
<section markdown="1">

## DevOps Tools
- Puppet
- Chef

A template for ntp config
```erb
driftfile /var/lib/ntp/drift
<% @boxes.each do |box| -%>
server <%= box.name -%><%= @ntp_server_suffix %>
<% end -%>

restrict -4 default kod notrap nomodify nopeer noquery
restrict -6 default kod notrap nomodify nopeer noquery
restrict 127.0.0.1
```

```
driftfile /var/lib/ntp/drift
server foo.ntp.cluster.org
server bar.ntp.cluster.org
server qux.ntp.cluster.org

restrict -4 default kod notrap nomodify nopeer noquery
restrict -6 default kod notrap nomodify nopeer noquery
restrict 127.0.0.1
```

</section>
<section markdown="1">

## Mail Merge
- Spam
- Reports

```
Dear <%= @employee.name %>,

You need to update your <%= report.type %> reports.
Come on in on  <%= Date::DAYNAMES[Date.today.next_day.wday] %> to finish those up.
```

```
Dear Peter Gibbons, 

You need to update your TPS reports.
Come on in on Saturday to finish those up.
```

[![Up arrow](https://s3.amazonaws.com/hakim-static/reveal-js/arrow.png){: style="transform: rotate(180deg);-webkit-transform: rotate(180deg);"}](#/2)

</section>
