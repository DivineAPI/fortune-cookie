
#################################
Fortune Cookie - DivineAPI
#################################
Start your FREE Trial to get your API KEY,  `https://divineapi.com <https://divineapi.com>`_

|travis| |Docs| |Maintenance yes| |SayThanks| |Paypal|
    
    
.. image:: https://divineapi.com/assets/images/logo.svg
   :height: 412px
   :width: 898px
   :alt: divineapi logo
   :align: center


What is Fortune Cookie API?
==============
Divine API is for those who are seeking for an excellently built Fortune Cookie API to
inculcate in their website or application. It extracts data to predict all about an Individuals
life and answers to the question he is seeking.

..
  Feel free to contribute on `Github <http://github.com/divineapi/horoscope-api>`_.




Why Fortune Cookie API?
==========
Divine API can help the developers to inculcate a finely built fortune cookie API and give
their customers a fun experience of cracking their own fortune cookie digitally.



Features
==========

- Fortune cookie API lets you crack your own fortune cookie digitally.
- It contains fortunes and quotes related to one’s lives.
- The attractive user interface captures customers interest greatly.
- Fun way to get the insights into future predictions.
- It answers to your questions that have remained unanswered for a while.


Benefits
==========

- Crack as many cookies as you want with the fortune cookie API.
- Receive the personalized fortune with the virtually baked fortune cookie.
- It shall bring vibrancy to your website.


URL
===
.. code-block:: python

    POST: https://divineapi.com/api/1.0/get_fortune_cookie.php


Parameters
==========

api_key : 
   Your API  KEY.


Result Example:
=====
.. code-block:: text


      {
          "success": 1,
          "message": "Fortune Cookie result.",
          "data": {
              "prediction": {
                  "result": "R1 new"
              }
          }
      }   


Example 
=======


cURL
^^^^
.. code-block:: curl

    curl -d "api_key=YOUR_API_KEY" -X POST https://divineapi.com/api/1.0/get_fortune_cookie.php


Python
^^^^^^
.. code-block:: python

   import requests
   from requests.structures import CaseInsensitiveDict

   url = "https://divineapi.com/api/1.0/get_fortune_cookie.php"

   headers = CaseInsensitiveDict()
   headers["Content-Type"] = "application/x-www-form-urlencoded"

   data = "api_key=YOUR_API_KEY"


   resp = requests.post(url, headers=headers, data=data)

   print(resp.status_code)


Javascript
^^^^^^^
.. code-block:: javascript

   var url = "https://divineapi.com/api/1.0/get_fortune_cookie.php";

   var xhr = new XMLHttpRequest();
   xhr.open("POST", url);

   xhr.setRequestHeader("Content-Type", "application/x-www-form-urlencoded");

   xhr.onreadystatechange = function () {
      if (xhr.readyState === 4) {
         console.log(xhr.status);
         console.log(xhr.responseText);
      }};

   var data = "api_key=YOUR_API_KEY";

   xhr.send(data);


PHP
^^^
.. code-block:: php

   <?php
    $url = "https://divineapi.com/api/1.0/get_fortune_cookie.php";

    $curl = curl_init($url);
    curl_setopt($curl, CURLOPT_URL, $url);
    curl_setopt($curl, CURLOPT_POST, true);
    curl_setopt($curl, CURLOPT_RETURNTRANSFER, true);

    $headers = array(
       "Content-Type: application/x-www-form-urlencoded",
    );
    curl_setopt($curl, CURLOPT_HTTPHEADER, $headers);

    $data = "api_key=YOUR_API_KEY";

    curl_setopt($curl, CURLOPT_POSTFIELDS, $data);

    $resp = curl_exec($curl);
    curl_close($curl);
    var_dump($resp);
   ?>
    
    
jQuery Ajax
^^^^^^
.. code-block:: javascript

    $.ajax({
   type:'POST',
   url:'https://divineapi.com/api/1.0/get_fortune_cookie.php',
   data: {api_key:'YOUR_API_KEY'},
   success:function(data){
   console.log(data);
   }
    });


ECMAScript (ES6)
^^^^^^
.. code-block:: javascript

    const URL = 'https://divineapi.com/api/1.0/get_fortune_cookie.php?api_key=YOUR_API_KEY';
    fetch(URL, {
        method: 'POST'
    })
    .then(response => response.json())
    .then(json => {
        const date = json.current_date;
        console.log(date);
    });


License
=======

2021 Divine API

Licensed under the Apache License, Version 2.0 (the "License");

    http://www.apache.org/licenses/LICENSE-2.0



Contact
=======

Questions? Suggestions? Feel free to contact me at admin@divineapi.com


Credits
=======

"DivineAPI" was created by `Azhar <https://azhar-spiderdev.github.io/portfolio>`_

Source of updates - https://divineapi.com/fortune-cookie-api

Please feel free to use and adapt this awesome API.

    
.. |Docs| image:: https://readthedocs.org/projects/aztro/badge/?version=latest
    :target: https://azhar-spiderdev.github.io/
    
.. |Maintenance yes| image:: https://img.shields.io/badge/Maintained%3F-yes-green.svg
   :target: https://azhar-spiderdev.github.io/


.. |Travis| image:: https://travis-ci.org/sameerkumar18/aztro.svg?branch=master
    :target: https://azhar-spiderdev.github.io/

.. |SayThanks| image:: https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg
    :target: https://azhar-spiderdev.github.io/

.. |Paypal| image:: https://img.shields.io/badge/Paypal-Donate-blue.svg
    :target: https://azhar-spiderdev.github.io/

.. Indices and tables
.. ==================

.. * :ref:`genindex`
.. * :ref:`modindex`
.. * :ref:`search`
