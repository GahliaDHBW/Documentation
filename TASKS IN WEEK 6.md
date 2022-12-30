# TASKS in WEEK 6: Let Code

After scraping the App should only request the URL to get the data, as seen in the following:

```js
import axios from "axios"
axios.get('https://port19x.github.io/mensascrap/master.json')
  .then(function (response) {
    // handle success
    console.table(response.data.body.erzbergerstraße.monday);
    console.table(response.data.body.erzbergerstraße.tuesday);
    console.table(response.data.body.erzbergerstraße.wednesday);
    console.table(response.data.body.erzbergerstraße.thursday);
    console.table(response.data.body.erzbergerstraße.friday);
  })
  .catch(function (error) {
    // handle error
    console.log(error);
  })
  .finally(function () {
    // always executed
  });
```
The Result

<img src =".\img\Scraping Result.png">

 **It is important to mention that, the display information are not equal to the real information, we just create our own sample / test data.** 

