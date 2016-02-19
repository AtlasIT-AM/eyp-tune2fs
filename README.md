# tune2fs

#### Table of Contents

1. [Overview](#overview)
2. [Module Description](#module-description)
3. [Setup](#setup)
    * [What tune2fs affects](#what-tune2fs-affects)
    * [Setup requirements](#setup-requirements)
    * [Beginning with tune2fs](#beginning-with-tune2fs)
4. [Usage](#usage)
5. [Reference](#reference)
5. [Limitations](#limitations)
6. [Development](#development)
    * [Contributing](#contributing)

## Overview

manages tune2fs attributes on a extfs

## Module Description

TODO

## Setup

### What tune2fs affects

TODO

### Setup Requirements

This module requires pluginsync enabled and eyp/nsswitch module installed

### Beginning with tune2fs

```puppet
tune2fs::extfs { '/dev/mapper/vg0-root':
  max_mount_count=>'30',
  reserved_blocks=> '0',
}
```

```puppet
tune2fs::extfs { '/dev/mapper/vg0-root':
  max_mount_count=>'30',
  reserved_blocks=> '20%',
}
```

## Usage

TODO

## Reference

TODO

## Limitations

TODO

## Development

We are pushing to have acceptance testing in place, so any new feature should
have some test to check both presence and absence of any feature

### Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
