Commerce Rules Physical
=======================

This Drupal 7 module adds more condition rules for Commerce Kickstart:

I. Order total weight comparison
II. Maximum product dimension comparison
III. The order contains shippable products

I only use the first condition on my project, other two are not tested yet
(code is based on patch #68 found on https://www.drupal.org/node/1344962).
Thank you deggertsen!

IMPORTANT NOTE: In order to make first condition to work for me, I had to write a custom
hook function to calculate order weight in case commerce_physical_order_weight
function returns NULL weight.
