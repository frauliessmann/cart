.. ==================================================
.. FOR YOUR INFORMATION
.. --------------------------------------------------
.. -*- coding: utf-8 -*- with BOM.

showCartAction-Konfiguration
============================

::

   plugin.tx_cart {
       settings {
           showCartAction {
               showPartials {
                   couponForm = true

                   # if setting shippingAddressForm to false please disable all validations too
                   shippingAddressForm = true

                   shippingMethodForm = true
                   paymentMethodForm = true
               }

               summary {
                   fields {
                       cart.net = true
                       cart.taxes = true
                       discount.gross = true
                       service.gross = true
                       total.gross = true
                   }
               }
           }
       }
   }

.. container:: table-row

   Property
      plugin.tx_cart.settings.showCartAction.showPartials.paymentMethodForm
   Data type
      boolean
   Description
      Aktiviert/Deaktiviert die Darstellung und Auswahl der konfigurierten Bezahlmethoden im Warenkorb.
   Default
      true

.. container:: table-row

   Property
      plugin.tx_cart.settings.showCartAction.showPartials.shippingMethodForm
   Data type
      boolean
   Description
      Aktiviert/Deaktiviert die Darstellung und Auswahl der konfigurierten Bezahlmethoden im Warenkorb.
   Default
      true

.. container:: table-row

   Property
      plugin.tx_cart.settings.showCartAction.showPartials.couponForm
   Data type
      boolean
   Description
      Aktiviert/Deaktiviert die Darstellung der Gutscheine im Warenkorb. Es wird sowohl der Block für die Eingabe als
      auch für die Darstellung ein-/ausgeblendet.
   Default
      true
