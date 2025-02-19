.. _sponsors:

================================================================================
Sponsors
================================================================================

GDAL is a truly collaborative effort, with many diverse organizations
contributing resources to its success. The following organizations take an
extra step, providing unrestricted funding every year to maintain and improve
the health of project:

- Platinium level:

  .. _platinium-sponsors:
  .. container:: horizontal-logos

    .. Note: they will appear in randomized order in HTML

    .. container:: horizontal-logo

        .. image:: ../../images/sponsors/logo-microsoft.png
           :class: img-logos
           :width: 250 px
           :target: https://www.microsoft.com

    .. container:: horizontal-logo

        .. image:: ../../images/sponsors/logo-planet.png
           :class: img-logos
           :width: 250 px
           :target: https://www.planet.com


- Gold level:

  .. _gold-sponsors:
  .. container:: horizontal-logos

    .. Note: they will appear in randomized order in HTML

    .. container:: horizontal-logo

        .. image:: ../../images/sponsors/logo-esri.png
           :class: img-logos
           :width: 200 px
           :target: https://www.esri.com

    .. container:: horizontal-logo

        .. image:: ../../images/sponsors/logo-google.png
           :class: img-logos
           :width: 200 px
           :target: https://www.google.com

    .. container:: horizontal-logo

        .. image:: ../../images/sponsors/logo-safe.png
           :class: img-logos
           :width: 200 px
           :target: https://www.safe.com



- Silver level:

  .. _silver-sponsors:
  .. container:: horizontal-logos

    .. Note: they will appear in randomized order in HTML

    .. container:: horizontal-logo

        .. image:: ../../images/sponsors/logo-koordinates.png
           :class: img-logos
           :width: 150 px
           :target: https://www.koordinates.com


    .. container:: horizontal-logo

        .. image:: ../../images/sponsors/logo-mapgears.png
           :class: img-logos
           :width: 150 px
           :target: https://www.mapgears.com


    .. container:: horizontal-logo

        .. image:: ../../images/sponsors/logo-sparkgeo.png
           :class: img-logos
           :width: 150 px
           :target: https://www.sparkgeo.com


- Supporter level:

    .. _supporter-sponsors:
    .. container:: horizontal-logos

      None listed yet.


.. raw:: html

   <script type="text/javascript">
    // Randomize logos
    $.fn.randomize = function(selector){
        var $elems = selector ? $(this).find(selector) : $(this).children(),
            $parents = $elems.parent();

        // found at: http://stackoverflow.com/a/2450976/746961
        function shuffle(array) {
            var currentIndex = array.length, temporaryValue, randomIndex;
            // While there remain elements to shuffle...
            while (0 !== currentIndex) {
                // Pick a remaining element...
                randomIndex = Math.floor(Math.random() * currentIndex);
                currentIndex -= 1;

                // And swap it with the current element.
                temporaryValue = array[currentIndex];
                array[currentIndex] = array[randomIndex];
                array[randomIndex] = temporaryValue;
            }
            return array;
        }

        $parents.each(function(){
            var elements = $(this).children(selector);
            shuffle(elements);
            $(this).append(elements);
        });

        return this;
    };
    $('#platinium-sponsors').randomize('div.horizontal-logo');
    $('#gold-sponsors').randomize('div.horizontal-logo');
    $('#silver-sponsors').randomize('div.horizontal-logo');
    $('#supporter-sponsors').randomize('div.horizontal-logo');
  </script>

The GDAL Project is hosted by `OSGeo <https://www.osgeo.org>`__, and
`NumFOCUS <https://numfocus.org>`__ will serve as the fiscal sponsor once GDAL's application is completed,
enabling all sponsorship to go through a 501(c)3 as charitable donations.

.. container:: horizontal-logos

    .. container:: horizontal-logo

        .. image:: ../../images/logo-osgeo.png
           :class: img-logos
           :width: 150 px
           :target: https://www.osgeo.org

    .. container:: horizontal-logo

        .. image:: ../../images/logo-numfocus.png
           :class: img-logos
           :width: 150 px
           :target: https://numfocus.org

Sponsoring
----------

If your organization benefits from GDAL we recommend joining the group of
sponsors above to "pay it forward" and ensure the project has the resources to
stay healthy and grow. To learn about the benefits of becoming a sponsor at
various levels start with the `Sustainable GDAL Sponsorship Prospectus`_.
If you are interested, need help convincing your key decision-makers, or have
any questions, don't hesitate to contact gdal-sponsors@osgeo.org.

Related resources
-----------------

- `Sustainable GDAL Sponsorship Prospectus`_.
- :ref:`Sponsoring frequently asked questions (FAQ) <sponsoring-faq>`.

.. _Sustainable GDAL Sponsorship Prospectus: https://gdal.org/sponsors/Sustainable%20GDAL%20Sponsorship%20Prospectus.pdf

..
    Developer comment: make html includes a hack to hide the table from
    the index.html file. We need to keep it visible so that the top-level
    index.html lists those pages.

.. toctree::
   :maxdepth: 0

   faq
