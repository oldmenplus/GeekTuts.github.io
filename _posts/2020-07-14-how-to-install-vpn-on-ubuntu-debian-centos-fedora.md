---
date: 2020-07-14T23:48:05.000Z
layout: post
title: How to Install OpenVPN on Ubuntu, Debian, CentOS, Fedora
subtitle: 'Install OpenVPN on Ubuntu, Debian, CentOS, Fedora'
description: >-
  This tutorial will guide you in setting up your own VPN.
  Installation of OpenVPN on Ubuntu, Debian, CentOS, Fedora.
image: >-
  https://res.cloudinary.com/dm7h7e8xj/image/upload/v1559821647/theme6_qeeojf.jpg
optimized_image: >-
  https://res.cloudinary.com/dm7h7e8xj/image/upload/c_scale,w_380/v1559821647/theme6_qeeojf.jpg
category: tutorial
tags:
  - ubuntu
  - debian
  - centos
  - fedora
  - openvpn
author: AmreshSinha     
paginate: true
---
# Why We Need a VPN?
Nowadays, censorship is becoming a pain for many normal web surfers, devolopers, etc.
Simple explanation to VPN is that it removes censorship!  
And if you want to dig more deep in its definition then visit this wikipedia page: [Virtual Private Network](https://en.wikipedia.org/wiki/Virtual_private_network)  
# Getting Started
Wait Wait! Before proceeding further I want to tell you about some freaking-awesome but cheap VPS providers which allows installation of VPN on their VPSes.
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Pricing</th>
      <th>Datacenters</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>Totals</td>
      <td>21</td>
      <td>23</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>[<img src="https://www.hostingadvice.com/images/uploads/2017/09/hostwinds.png?width=175&height=55">](https://hostwinds.com/)</td>
      <td>$4.49/month(managed)  
        $5.17(managed)</td>
      <td>11</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <td>Charlie</td>
      <td>7</td>
      <td>9</td>
    </tr>
  </tbody>
</table>
[Hostwinds](https://www.hostwinds.com/vps/)
  * Pricing Starts from: $4.49/month(managed) or $5.17(managed)  
  * It has few data-centers: In Seattle, Dallas, Amsterdam <br />
 [VPSServer](https://www.vpsserver.com/)  
  * Pricing Starts from: $4.99/month(managed)
  * It has many data-centers: In USA, Europe, Asia, Australia 
Etiam porta **sem malesuada magna** mollis euismod. Cras mattis consectetur purus sit amet fermentum. Aenean lacinia bibendum nulla sed consectetur.

## Inline HTML elements

HTML defines a long list of available inline tags, a complete list of which can be found on the [Mozilla Developer Network](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).

* **To bold text**, use `<strong>`.
* *To italicize text*, use `<em>`.
* Abbreviations, like <abbr title="HyperText Markup Langage">HTML</abbr> should use `<abbr>`, with an optional `title` attribute for the full phrase.
* Citations, like <cite>&mdash; Thiago Rossener</cite>, should use `<cite>`.
* <del>Deleted</del> text should use `<del>` and <ins>inserted</ins> text should use `<ins>`.
* Superscript <sup>text</sup> uses `<sup>` and subscript <sub>text</sub> uses `<sub>`.

Most of these elements are styled by browsers with few modifications on our part.

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

Vivamus sagittis lacus vel augue rutrum faucibus dolor auctor. Duis mollis, est non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem nec elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.

--page-break--

## Code

Cum sociis natoque penatibus et magnis dis `code element` montes, nascetur ridiculus mus.

```js
// Example can be run directly in your JavaScript console

// Create a function that takes two arguments and returns the sum of those arguments
var adder = new Function("a", "b", "return a + b");

// Call the function
adder(2, 6);
// > 8
```

Aenean lacinia bibendum nulla sed consectetur. Etiam porta sem malesuada magna mollis euismod. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa.

## Lists

Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Aenean lacinia bibendum nulla sed consectetur. Etiam porta sem malesuada magna mollis euismod. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.

* Praesent commodo cursus magna, vel scelerisque nisl consectetur et.
* Donec id elit non mi porta gravida at eget metus.
* Nulla vitae elit libero, a pharetra augue.

Donec ullamcorper nulla non metus auctor fringilla. Nulla vitae elit libero, a pharetra augue.

1. Vestibulum id ligula porta felis euismod semper.
2. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
3. Maecenas sed diam eget risus varius blandit sit amet non magna.

Cras mattis consectetur purus sit amet fermentum. Sed posuere consectetur est at lobortis.

Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Nullam quis risus eget urna mollis ornare vel eu leo.

## Images

Quisque consequat sapien eget quam rhoncus, sit amet laoreet diam tempus. Aliquam aliquam metus erat, a pulvinar turpis suscipit at.

![placeholder](https://placehold.it/800x400 "Large example image") ![placeholder](https://placehold.it/400x200 "Medium example image") ![placeholder](https://placehold.it/200x200 "Small example image")

## Tables

Aenean lacinia bibendum nulla sed consectetur. Lorem ipsum dolor sit amet, consectetur adipiscing elit.

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Upvotes</th>
      <th>Downvotes</th>
    </tr>
  </thead>
  <tfoot>
    <tr>
      <td>Totals</td>
      <td>21</td>
      <td>23</td>
    </tr>
  </tfoot>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>10</td>
      <td>11</td>
    </tr>
    <tr>
      <td>Bob</td>
      <td>4</td>
      <td>3</td>
    </tr>
    <tr>
      <td>Charlie</td>
      <td>7</td>
      <td>9</td>
    </tr>
  </tbody>
</table>

Nullam id dolor id nibh ultricies vehicula ut id elit. Sed posuere consectetur est at lobortis. Nullam quis risus eget urna mollis ornare vel eu leo.
