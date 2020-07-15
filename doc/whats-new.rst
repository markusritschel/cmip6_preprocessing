.. currentmodule:: cmip6_preprocessing

What's New
===========

.. _whats-new.0.2.0:

v0.2.0 (unreleased)
---------------------

Breaking changes
~~~~~~~~~~~~~~~~
- Consistent treatment of cf-style bounds. The combination of `parse_lon_lat_bounds`,
`maybe_convert_bounds_to_vertex`, `maybe_convert_vertex_to_bounds`, and `sort_vertex_order` applied on the dataset, assures
that all datasets have both conventions available and the vertex order is the same.
By `Julius Busecke <https://github.com/jbusecke>`_

- New implementation of `replace_x_y_nominal_lat_lon`, which avoids duplicate values in the derived dimensions (:issue:`34`) (:pull:`35`)
By `Julius Busecke <https://github.com/jbusecke>`_

New Features
~~~~~~~~~~~~
- Create merged region masks with :py:func:`merged_mask` (:pull:`18`)
  By `Julius Busecke <https://github.com/jbusecke>`_


Bug fixes
~~~~~~~~~


Documentation
~~~~~~~~~~~~~


Internal Changes
~~~~~~~~~~~~~~~~
-  Add `ni` and `nj` to the `rename_dict` dictionary in _preprocessing.py_ as dimensions to be corrected (:pull:`54`)
   By `Markus Ritschel <https://github.com/markusritschel>`_


.. _whats-new.0.1.2:

v0.1.2
---------------------


New Features
~~~~~~~~~~~~
- Added more models, now supporting both ocean and atmospheric output for :py:func:`combined_preprocessing` (:pull:`14`)
  By `Julius Busecke <https://github.com/jbusecke>`_



.. _whats-new.0.1.0:

v0.1.0 (2/21/2020)
----------------------

Initial release.
