# Reference

<!-- DO NOT EDIT: This document was generated by Puppet Strings -->

## Table of Contents

### Functions

* [`dns_a`](#dns_a): [DEPRECATED] Retrieves DNS A records for a domain and returns them as an array.
* [`dns_aaaa`](#dns_aaaa): [DEPRECATED] Retrieves DNS AAAA records for a domain and them it as an array.
* [`dns_cname`](#dns_cname): [DEPRECATED] Retrieves a DNS CNAME record for a domain and returns it as a string.
* [`dns_lookup`](#dns_lookup): [DEPRECATED] Do a DNS lookup and returns an array of addresses. This will follow CNAMEs and return any matching IPv4 or IPv6 addresses. See t
* [`dns_mx`](#dns_mx): [DEPRECATED] Retrieves DNS MX records for a domain and returns them as an array.
* [`dns_ptr`](#dns_ptr): [DEPRECATED] Retrieves DNS PTR records for a domain and returns them as an array.
* [`dns_srv`](#dns_srv): [DEPRECATED] Retirve the SRV domain for a specific domain
* [`dns_txt`](#dns_txt): [DEPRECATED] Retrieves DNS TXT records for a domain and as an array.
* [`dnsquery::a`](#dnsquery--a): Retrieves DNS A records for a domain and returns them as an array.
* [`dnsquery::aaaa`](#dnsquery--aaaa): Retrieves DNS AAAA records for a domain and them it as an array.
* [`dnsquery::cname`](#dnsquery--cname): Retrieves a DNS CNAME record for a domain and returns it as a string.
* [`dnsquery::lookup`](#dnsquery--lookup): Do a DNS lookup and returns an array of addresses. This will follow CNAMEs and return any matching IPv4 or IPv6 addresses. See the more speci
* [`dnsquery::mx`](#dnsquery--mx): Retrieves DNS MX records for a domain and returns them as an array.
* [`dnsquery::ptr`](#dnsquery--ptr): Retrieves DNS PTR records for a domain and returns them as an array.
* [`dnsquery::rlookup`](#dnsquery--rlookup): Retrieves results from DNS reverse lookup and returns it as an array.
* [`dnsquery::soa`](#dnsquery--soa): Retrieves DNS SOA records and returns it as a hash.
* [`dnsquery::srv`](#dnsquery--srv): Retirve the SRV domain for a specific domain
* [`dnsquery::txt`](#dnsquery--txt): Retrieves DNS TXT records for a domain and return as an array.

### Data types

* [`Dnsquery::Mx`](#Dnsquery--Mx): type used for DNS MX records
* [`Dnsquery::Soa`](#Dnsquery--Soa): type used for DNS SOA records
* [`Dnsquery::Srv`](#Dnsquery--Srv): type used for DNS SRV records

## Functions

### <a name="dns_a"></a>`dns_a`

Type: Ruby 4.x API

[DEPRECATED] Retrieves DNS A records for a domain and returns them as an array.

#### `dns_a(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

[DEPRECATED] Retrieves DNS A records for a domain and returns them as an array.

Returns: `Array[Stdlib::IP::Address::V4::Nosubnet]` An array of A answers matching domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dns_aaaa"></a>`dns_aaaa`

Type: Ruby 4.x API

[DEPRECATED] Retrieves DNS AAAA records for a domain and them it as an array.

#### `dns_aaaa(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

[DEPRECATED] Retrieves DNS AAAA records for a domain and them it as an array.

Returns: `Array[Stdlib::IP::Address::V6::Nosubnet]` An array of AAAA records matching domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dns_cname"></a>`dns_cname`

Type: Ruby 4.x API

[DEPRECATED] Retrieves a DNS CNAME record for a domain and returns it as a string.

#### `dns_cname(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

[DEPRECATED] Retrieves a DNS CNAME record for a domain and returns it as a string.

Returns: `Stdlib::Fqdn` An string representing the CNAME of a domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dns_lookup"></a>`dns_lookup`

Type: Ruby 4.x API

[DEPRECATED] Do a DNS lookup and returns an array of addresses.
This will follow CNAMEs and return any matching IPv4 or IPv6 addresses.
See the more specific functions if you only want one type returned.

#### `dns_lookup(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

[DEPRECATED] Do a DNS lookup and returns an array of addresses.
This will follow CNAMEs and return any matching IPv4 or IPv6 addresses.
See the more specific functions if you only want one type returned.

Returns: `Array[Stdlib::IP::Address::Nosubnet]` An array of A and AAAA answers matching domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dns_mx"></a>`dns_mx`

Type: Ruby 4.x API

[DEPRECATED] Retrieves DNS MX records for a domain and returns them as an array.

#### `dns_mx(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

[DEPRECATED] Retrieves DNS MX records for a domain and returns them as an array.

Returns: `Array[Dnsquery::Mx]` An array of hashes representing the mx records for domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dns_ptr"></a>`dns_ptr`

Type: Ruby 4.x API

[DEPRECATED] Retrieves DNS PTR records for a domain and returns them as an array.

#### `dns_ptr(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

[DEPRECATED] Retrieves DNS PTR records for a domain and returns them as an array.

Returns: `Array[Stdlib::Fqdn]` An array of PTR answeres matching domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dns_srv"></a>`dns_srv`

Type: Ruby 4.x API

[DEPRECATED] Retirve the SRV domain for a specific domain

#### `dns_srv(String $domain, Optional[Callable] &$block)`

[DEPRECATED] Retirve the SRV domain for a specific domain

Returns: `Array[Dnsquery::Srv]` The srv records for domain as an array of hashs

##### `domain`

Data type: `String`

the dns question to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dns_txt"></a>`dns_txt`

Type: Ruby 4.x API

[DEPRECATED] Retrieves DNS TXT records for a domain and as an array.

#### `dns_txt(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

[DEPRECATED] Retrieves DNS TXT records for a domain and as an array.

Returns: `Array[Array[String]]` The txt record for a domain as an array

##### `domain`

Data type: `Stdlib::Fqdn`

the dns question to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--a"></a>`dnsquery::a`

Type: Ruby 4.x API

Retrieves DNS A records for a domain and returns them as an array.

#### `dnsquery::a(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

Retrieves DNS A records for a domain and returns them as an array.

Returns: `Array[Stdlib::IP::Address::V4::Nosubnet]` An array of A answers matching domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--aaaa"></a>`dnsquery::aaaa`

Type: Ruby 4.x API

Retrieves DNS AAAA records for a domain and them it as an array.

#### `dnsquery::aaaa(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

Retrieves DNS AAAA records for a domain and them it as an array.

Returns: `Array[Stdlib::IP::Address::V6::Nosubnet]` An array of AAAA records matching domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--cname"></a>`dnsquery::cname`

Type: Ruby 4.x API

Retrieves a DNS CNAME record for a domain and returns it as a string.

#### `dnsquery::cname(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

Retrieves a DNS CNAME record for a domain and returns it as a string.

Returns: `String` An string representing the CNAME of a domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--lookup"></a>`dnsquery::lookup`

Type: Ruby 4.x API

Do a DNS lookup and returns an array of addresses.
This will follow CNAMEs and return any matching IPv4 or IPv6 addresses.
See the more specific functions if you only want one type returned.

#### `dnsquery::lookup(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

Do a DNS lookup and returns an array of addresses.
This will follow CNAMEs and return any matching IPv4 or IPv6 addresses.
See the more specific functions if you only want one type returned.

Returns: `Array[Stdlib::IP::Address::Nosubnet]` An array of A and AAAA answers matching domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--mx"></a>`dnsquery::mx`

Type: Ruby 4.x API

Retrieves DNS MX records for a domain and returns them as an array.

#### `dnsquery::mx(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

Retrieves DNS MX records for a domain and returns them as an array.

Returns: `Array[Dnsquery::Mx]` An array of hashes representing the mx records for domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--ptr"></a>`dnsquery::ptr`

Type: Ruby 4.x API

Retrieves DNS PTR records for a domain and returns them as an array.

#### `dnsquery::ptr(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

Retrieves DNS PTR records for a domain and returns them as an array.

Returns: `Array[Stdlib::Fqdn]` An array of PTR answeres matching domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns domain to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--rlookup"></a>`dnsquery::rlookup`

Type: Ruby 4.x API

Retrieves results from DNS reverse lookup and returns it as an array.

#### `dnsquery::rlookup(Stdlib::IP::Address::Nosubnet $address, Optional[Callable] &$block)`

Retrieves results from DNS reverse lookup and returns it as an array.

Returns: `Array[Stdlib::Fqdn]` An array of hostnames matching the ip address

##### `address`

Data type: `Stdlib::IP::Address::Nosubnet`

the ip address to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--soa"></a>`dnsquery::soa`

Type: Ruby 4.x API

Retrieves DNS SOA records and returns it as a hash.

#### `dnsquery::soa(Stdlib::Fqdn $question, Optional[Callable] &$block)`

Retrieves DNS SOA records and returns it as a hash.

Returns: `Dnsquery::Soa` The SOA record matching domain

##### `question`

Data type: `Stdlib::Fqdn`

the dns question to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--srv"></a>`dnsquery::srv`

Type: Ruby 4.x API

Retirve the SRV domain for a specific domain

#### `dnsquery::srv(String $domain, Optional[Callable] &$block)`

Retirve the SRV domain for a specific domain

Returns: `Array[Dnsquery::Srv]` The srv records for domain as an array of hashs

##### `domain`

Data type: `String`

the dns question to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

### <a name="dnsquery--txt"></a>`dnsquery::txt`

Type: Ruby 4.x API

Retrieves DNS TXT records for a domain and return as an array.

#### `dnsquery::txt(Stdlib::Fqdn $domain, Optional[Callable] &$block)`

Retrieves DNS TXT records for a domain and return as an array.

Returns: `Array[Array[String]]` The txt domain for a domain

##### `domain`

Data type: `Stdlib::Fqdn`

the dns question to lookup

##### `&block`

Data type: `Optional[Callable]`

an optional lambda to return a default value in case the lookup fails

## Data types

### <a name="Dnsquery--Mx"></a>`Dnsquery::Mx`

type used for DNS MX records

Alias of

```puppet
Struct[{
  preference => Integer[0,65535],
  exchange   => Stdlib::Fqdn,
}]
```

### <a name="Dnsquery--Soa"></a>`Dnsquery::Soa`

type used for DNS SOA records

Alias of

```puppet
Struct[{
  mname   => Stdlib::Fqdn,
  rname   => Stdlib::Fqdn,
  expire  => Integer,
  minimum => Integer,
  refresh => Integer,
  retry   => Integer,
  serial  => Integer,
}]
```

### <a name="Dnsquery--Srv"></a>`Dnsquery::Srv`

type used for DNS SRV records

Alias of

```puppet
Struct[{
  priority => Integer[0,65535],
  weight   => Integer[0,65535],
  port     => Stdlib::Port,
  target   => Stdlib::Fqdn,
}]
```
