# <strong style="text-align: center">বিড়ালদের জাভাস্ক্রিপ্ট</strong>
## নতুনদের জন্য প্রোগ্রামিংয়ের সূচনা ![cat](images/substack-cats.png)
### *এতই সহজ যে তোমার মনুষ্য সঙ্গীও বুঝতে পারবে!*

জাভাস্ক্রিপ্ট হলো একটা প্রোগ্রামিং ভাষা, অন্যভাবে বলতে গেলে এমন একটি উপায় যা দিয়ে কম্পিউটারকে বিভিন্ন কাজ করতে আদেশ দেয়া যায়। ঠিক যেভাবে তুমি একটা মানুষকে তোমার ভাষায় মিউ মিউ করে আদেশ করো, তেমনভাবেই কম্পিউটারকে একটি প্রোগ্রামিং ভাষায় লিখিতভাবে কম্পিউটারকে কন্ট্রোল করতে পারবে। সব ব্রাউজারই জাভাস্ক্রিপ্ট বুঝতে পারে, আর তুমি সেই সুযোগ কাজে লাগিয়ে অসাধারণ সবকিছু করতে পারবে।

জাভাস্ক্রিপ্টের শুরুটা হয়েছিলো ওয়েবপেজ গুলো ইন্টারেক্টিভ করার জন্য। কিন্তু এখন জাভাস্ক্রিপ্ট শুধু ব্রাউজারেই চলে না, এটা সার্ভার, মোবাইল এবং এমনকি রোবোটেও চলে। এই পেজে তুমি জাভাস্ক্রিপ্টের বেসিক শিখতে পারবে, যাতে তুমিও অল্প সময়েই শুরু করতে পারো।

*সত্যি বলতে একদমই সময় লাগবে না, কিংবা হয়তো দুই এক ঘন্টা লাগবে, কিন্তু তুমি যেহেতু একটি বিড়াল, তাই তোমার দৌড়াদৌড়ির সম্ভাবনা কম, এবং রোদ পোহানোর সম্ভাবনা বেশি, নাহয় ওই সময়টাই কাজে লাগালে।*

## সূচীপত্র

- [কনসোল](#basics)
- [স্ট্রিং](#strings)
- [ভ্যালু আর ভ্যারিয়েবল](#values)
- [ফাংশন](#functions)
- [জাভাস্ক্রিপ্টের ভিতরের ফাংশনগুলো](#standard-library)
- [নতুন ফাংশন ডাউনলোড করা](#third-party-javascript)
- [নতুন ফাংশন লেখা](#writing-functions)
- [লুপ](#loops)
- [এরে](#arrays)
- [অবজেক্ট](#objects)
- [কলব্যাক](#callbacks)
- [আরো জানতে যা পড়বে](#recommended-reading)

## ভয় পেলে চলবে না

![cat](images/yarnify.png)

তোমাকে সর্বোদাই নিজের পায়ে চলতে হবে &mdash; এমনকি প্রোগ্রামিং এর ক্ষেত্রেও ঠিক তাই! এই টিউটোরিয়াল কোনোভাবেই তোমার কম্পিউটার কে নষ্ট করবে না। একগ্লাস পানি যখন তোমার কম্পিউটারের উপর পড়ে তখন তোমার কম্পিউটার নষ্ট হয়ে যায়। কিন্তু তুমি যদি কমান্ড টাইপ করতেও ভুল করো তাও তোমার কম্পিউটারের কিছুই হবেনা। বড়জোড় তোমার কম্পিউটারের ব্রাউজারকে রিফ্রেশ দেয়া লাগতে পারে। বিড়ালের মত, কম্পিউটার প্রোগ্রামার রাও সবসময় ভুল করে। যেমন: টাইপিং মিস্টেক, উক্তিচিহ্ন বা ব্রাকেটে ভুল করা, এবং কিভাবে বেসিক ফাংশনগুলো (ইয়ার্ন, লেজার) ইত্যাদি কিভাবে কাজ করে। প্রোগ্রামাররা কোনোকিছু তৈরি করলে সেটাকে এমনভাবে তৈরি করে যেনো সেটা প্রথমবার কাজে না এসে পুর্ণাঙ্গভাবে কাজে লাগে। আসলে শেখার সেরা উপায় হলো ভুল করা।

সুতরাং ভিতু বেড়াল সাজলে চলবে না। যদি ভুল হয়েও যায়, তাহলে সর্বোচ্চ ব্রাউজারের যে পেইজে তুমি কাজ করছো সেই পেজটি রিফ্রেশ দেয়া লাগতে পারে। ভয় পাওয়ার কিছুই নেই। এটা খুবই কম ঘটে।

## <a id="basics" href="#basics">#</a> কনসোল

বর্তমানে এই পেইজে জাভাস্ক্রিপ্ট কাজ করছে। চলো এর সাথে একটু খেলা করা যাক। সাধারনত সহজতার ক্ষেত্রে আমি মনে করছি তুমি এই পেজ টি গুগল ক্রোম ব্যবহার করে ব্রাউজ করছো (কেননা এতে আমাদের দুজনেরই সুবিধা হবে যদি তুমিও ক্রোম ব্যবহার করো)।

প্রথমে, স্ক্রীনের যেকোনো জায়গায় মাউসের রাইট বাটন ক্লিক করো এবং নতুন যেই পপআপ মেন্যু আসবে সেখান থেকে **Inspect Element** সিলেক্ট করো, তারপর **Console** নামক ট্যাবে ক্লিক করো। তুমি অনেকটা এমন দেখতে পাবে:

![console](images/console.gif)

এটা হলো কনসোল, অন্যভাবে তুমি এটাকে কমান্ড লাইন বা টার্মিনাল হিসেবে ভাবতে পারো। আসলে এটা দিয়ে তুমি কম্পিউটারে যেই কমান্ড দেবে সেই কমান্ড ই ইনিস্ট্যান্টলি রিপ্লাই দেয়ার একটা মাধ্যম। কনসোল শেখার জন্য ব্যবহার করা টুলসগুলোর ভিতরে সবচেয়ে জনপ্রিয় ও ব্যবহৃত (আমি এখনো প্রায় প্রতিদিনই কোডিং করার সময় কনসোল ব্যবহার করে থাকি)।

কনসোলের কিছু চমৎকার ভালো দিক আছে। যেমন আমি যদি কিছু কনসোলে টাইপ করি তাহলে কনসোল আমাকে সেই শব্দ বা কমান্ডকে সম্পুর্ন করার জন্য সম্ভাব্য কমান্ডের একটি লিস্ট শো করে। আরেকটা মজার জিনিস, তুমি কনসোলে `1 + 1` টাইপ করো এবং `Enter` কী প্রেশ করে দেখো কি হয়।

কনসোলের ব্যবহার জাভাস্ক্রীপ্ট শেখার অন্যতম গুরুত্বপুর্ণ একটি পার্ট। যদি তুমি না যানো যে, তোমার কমান্ড কাজ করবে কিনা বা তোমার কমান্ডে কি কাজ হবে তবে কনসোল তোমাকে এক্ষেত্রে সম্পুর্ণ সাহায্য করবে। একটি উদাহরন দেয়া হলোঃ

### <a id="strings" href="#strings">#</a> স্ট্রিং

যেহেতু আমি একটি বিড়াল তাই আমি চাচ্ছি যে, ইন্টারনেটে থাকা সকল উদাহরনগুলের থেকে `dog` শব্দটির পরিবর্তে `those blasted dogs` বসাতে। প্রথমে তোমার কনসোলে যাও। তারপর `dog` শব্দটি অন্ততপক্ষে একবার আছে এমন একটি বাক্য লিখ। জাভাস্ক্রিপ্টে কতোগুলো শব্দ, বর্ণ, নম্বর বা যেকোনোকিছুকেই **String** হিসেবে ধরা হয় (এমনকি অক্ষরকেও *string* ধরা হয়)। স্ট্রিং শুরু ও শেষ হয় কোটেশন মার্ক দ্বারা। তুমি চাইলে সিঙ্গেল কোটেশন মার্ক `'` বা ডাবল কোটেশন মার্ক `"` যেটা ইচ্ছা ব্যবাহর করতে পারো তবে, একটা ব্যপারে খেয়াল রাখবে যে তুমি শুরু যা দিয়ে করবে শেষেও ঠিক তাই বসাবে।

![console](images/console-strings.gif)

বিদঘুটে ইরোরটা লক্ষ্য করেছো? ভয় পেয়োনা - তুমি কোনো আইন ভঙ্গ করোনি। SyntaxError ILLEGAL তখনই দেখায় যখন রোবোট তোমার প্রোগ্রামে ভুল খুজে পায়। প্রথম দুটি বাক্যের শুরুতে এবং শেষে একই কোটেশন মার্ক ব্যবহার করায় তাদের ক্ষেত্রে কোনো ইরোর দেখায় নি। কিন্তু যখনই আমি দুটোকে একত্রে ব্যবহার করতে চাই তখনই বিপত্তিটা আসল ঘটে।

আচ্ছা, উপরের উদাহরনগুলো থেকে যেকোনো একটা বাক্যকে সঠিক করতে (বাক্য `dog` শব্দটির পরিবর্তে আমাদের নিরবাচিত শব্দ বসাতে) আমাদের প্রথমে মুল বাক্যটাকে সংরক্ষন করে রাখতে হবে যাতে পরে আমরা তাকে কল করতে পারি এবং আমাদের পরিবর্তনের জাদু দেখাতে পারি। একটা ব্যাপার লক্ষ্য করো যখনই আমরা কনসোলে স্ট্রিং টাইপ করি তখনই তা দিত্বীয়বার লাল রংয়ের হয়ে পুনরাবৃত্তি করে? এর কারন হলো আমরা কম্পিউটারকে বলি নাই যে বাক্যটি সংরক্ষন করে রাখো। তাই এটি সাথে সাথেই আমাদের আউটপুট করে দেয়(অথবা এটি ইরোর দেখায় যদি আমরা কোথায় ভুল করে থাকি)।

### <a id="values" href="#values">#</a> Values and variables

**Values** are the simplest components in JavaScript. `1` is a value, `true` is a value, `"hello"` is a value, `function() {}` is a value, the list goes on! There are a handful of different **types** of values in JavaScript but we don't need to go over them all right away &mdash; you will learn them naturally the more you code!

To store values we use things called **variables**. The word 'variable' means 'can change' and is used because variables can store many different types of values and can change their value many times. They are pretty much like mailboxes. We put something in a variable, like our sentence, and then give the variable an address that we can use to look up the sentence later. In real life mailboxes have to have PO Box numbers but in JavaScript you usually just use lowercase letters or numbers without any spaces.

![console](images/console-variables.gif)

`var` is shorthand for variable and the `=` means *store the thing on the right-hand side in the thing on the left-hand side*. Also as you can see, now that we are storing our sentence in a variable the console doesn't just return our sentence right away, but instead gives us `undefined` which means *there was nothing to return*.

If you simply type a variable name into the console it will print out the value stored in that variable. A note about variables is that by default they go away when you switch to a different page. If I were to hit the Refresh button in Chrome, for example, my `dogSentence` variable would get wiped and it would be like it never existed. But don't worry about this too much for now &mdash; you can just hit the up or down arrows on your keyboard while in the console to go through everything you've entered in recently.

  

### <a id="functions" href="#functions">#</a> ফাংশন'স

এখন আমাদের বাক্যগুলো  ভ্যারিয়েবেল এর মধ্যে সংরক্ষিত আছে ,চলো আমরা এটিতে সংরক্ষিত একটি শব্দ পরিবর্তন  করি ! আমরা একটি  ফাংশন ব্যবহার করে এই কাজটি সম্পন্ন করতে পারি । ফাংশন  হল এক ধরনের মান যা, ভালোভাবে , একটি নির্দিষ্ট ফাংশনকে পরিবেশন করে (অন্য ভাবে বললে, উদ্দেশ্য অথবা কাজ )  আমাদের জন্য । তাদেরকে "ক্রিয়াকাণ্ড" নামে ডাকলে  একটু অদ্ভহুত শোনা যায়, আমি মনে করি এর জন্যই তারা এই নামের  পরিবর্তে "ফাংশন" নামে চলে গিয়েছে ।   

জাভাস্ক্রিপ্টে একটি ফাংশন আছে  `replace`  নামে  ঠিক  যেমন টা আমরা চাই ! ফাংশন তার বন্ধনিগুলিতে যেকোনো সংখ্যক মান নেয় (০, ১ অথবা এর অধিক) এবং  (`undefined`)   অথবা পরিবর্তিত স্ট্রিং ছাড়া কিছুই ফেরত দেয় না । (`Replace`) ফাংশন  যেকোনো স্ট্রিং এই সচরাচর  ব্যবহার করা যায়  এবং ২ টা মান লাগেঃ  অক্ষরগুলো সংগ্রহ করা এবং অক্ষরগুলো বিনিময় করা। এটা বর্ণনা করতে গেলে বিষয়গুলো গুলিয়ে যেতে পারে তাই এখানে উদাহরন দিয়ে দেখানো হলঃ

![console](images/console-replace.gif)

লক্ষ্য  করেছো  কিভাবে `dogSentence`   এর মান একই রয়েছে , এমন কি আমরা  এর উপর `replace`  ব্যবহার করার পরেও ? তার কারন হচ্ছে   `replace`  ফাংশন ( এবং বেশিরভাগ  জাভাস্ক্রিপ্ট ফাংশনের ক্ষেত্রেও একই ) আমরা যেই মান দেই তা সে নেয় এবং ফেরত দেয় একটি নতুন মান , কোনোরূপ  মান পরিবর্তন করা ছাড়াই যা আমরা দিয়েছি । যেহেতু আমরা কোন  ফলাফল সংরক্ষন করিনি ( ` replace`  ফাংশন এর  বাম দিকে কোন `=`  নেই  ) এটা শুধু মুদ্রিত করবে কনসোলে যে মান রিটার্ন করা হয়েছে।


### <a id="standard-library" href="#standard-library">#</a> স্ট্যান্ডার্ড লাইব্রেরি

তোমরা অবাক হতে পারো এই ভেবে যে আরও কি ধরনের ফাংশন রয়েছে জাভাস্ক্রিপ্টে। উত্তরটা হবেঃ এক টন। প্রচুর পরিমান তৈরিকৃত, স্ট্যান্ডার্ড লাইব্রেরি রয়েছে যা তুমি শিখতে পারবে MDN থেকে (মজিলা দ্বারা পরিচালিত একটি সাইট যেখানে ওয়েব টেকনোলজি সম্পর্কে প্রচুর তথ্য রয়েছে)। উদাহরণস্বরূপ, [এই হল MDN পেইজে জাভাস্ক্রিপ্টের ম্যাথ অবজেক্ট](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math).

### <a id="third-party-javascript" href="#third-party-javascript">#</a> থার্ড -পার্টি  জাভাস্ক্রিপ্ট

এমন অনেক জাভাস্ক্রিপ্ট কোড রয়েছে যা তৈরি নেই । জাভাস্ক্রিপ্টে থার্ড পার্টিস অর্থাৎ তৃতীয় পক্ষ হতে একটি "লাইব্রেরি" বা "প্লাগইন" হিসাবে উল্লেখ করা হয়। আমার প্রিয় একটির নাম হল `Underscore.js`। চলো আমরা এটি ধরি এবং আমাদের পেইজে এটি লোড করি! প্রথমে যাবো underscore সাইটে ,  ( http://underscorejs.org/) ,  ডাউনলোড  লিঙ্কে ক্লিক করতে হবে ( আমি সাধারনত ব্যবহার করি ডেভেলপমেন্ট ভার্সন কারন এগুলো পড়তে সহজ কিন্তু উভয়ই আপনাকে একই বেসিক ফাংশনালিটি প্রদান করবে), এবং এরপর সব কোড কপি করে তোমার ক্লিপবোর্ডে রাখো (তুমি এডিট মেনু থেকে সিলেক্ট অল ব্যবহার করে সবকিছু সিলেক্ট করতে পারবে)। তারপর তোমার কনসোলের মধ্যে এটি পেস্ট করো এবং এন্টার প্রেস করো । এখন তোমার ব্রাউজারে একটি নতুন ভ্যারিয়াবেল যোগ হয়েছেঃ `_` Underscore তোমাকে অনেক সুবিধা প্রদান করবে ফাংশনের সাথে খেলা করতে । আমরা পরে আরও শিখব কিভাবে এগুলো ব্যবহার করতে হয়।   

  ![console](images/underscore.gif)

### <a id="writing-functions" href="#writing-functions">#</a> নতুন ফাংশন তৈরি 

তুমি অন্য মানুষের তৈরিকৃত ফাংশন ব্যবহারে সীমাবদ্ধ থাকবে না - তুমি নিজেও এমন লিখতে পারবে। এটি খুবই সহজ! চলো তাহলে আমরা `makeMoreExciting` নামের একটি ফাংশন তৈরি করি যেখানে বিস্ময়বোধক চিহ্ন যোগ হবে স্ট্রিং এর শেষে।

```js
function makeMoreExciting(string) {
    return string + '!!!!'
} 
```

  আমার মাথার ভেতরে  আমি এইভাবে জোরে জোরে পড়ি: "এমন একটি ফাংশন আছে যা 'আরো উত্তেজনাপূর্ণ করে'  যা একটি স্ট্রিং নেয় এবং সেই স্ট্রিং এর একটি নতুন কপি ফেরত দেয় যার শেষে বিস্ময়বোধক চিহ্নের একটি গুচ্ছ আছে"। এখানে আমরা কীভাবে ম্যানুয়ালি কনসোল লিখতে পারি যদি আমরা ফাংশন ব্যবহার না করি:

![console](images/custom-function-manually.gif)


এক্সপ্রেশন স্ট্রিং + '!!!!' একটি নতুন স্ট্রিং ফেরৎ দেয়  এবং আমাদের ভেরিয়েবল নামক স্ট্রিংটি আগের মতোই থাকে (যেহেতু আমরা এটির `=`সাথে অন্য কোনও কিছু আপডেট করি নি  ) ।


চলো আমরা এটা ম্যানুয়ালি করার পরিবর্তে ফাংশন ব্যবহার করি । প্রথমে, ফাংশনটি কন্সোলের মধ্যে পেস্ট করব এবং তারপর ফাংশন্ কল করবো স্ট্রিং চালানোর মধ্য দিয়ে:  

 ![console](images/custom-function-call.gif)

তুমি একটি ভেরিয়েবেলের মাধ্যমে একই ফাংশন কল করতে পারবে যা একটি স্ট্রিং নির্দেশ করে (উপরের উদাহরণে আমরা কেবল একটি ভেরিয়েবেলকে সংরক্ষণ করার পরিবর্তে মান হিসাবে স্ট্রিংটি টাইপ করেছি):  
 
![console](images/custom-function-call-variable.gif)

 `makeMoreExciting(sentence)`  লাইনটি  সহজভাবে বললে হয়  `sentence + '!!!!'` । কি হতো যদি আমরা  
বাক্যটির মানের জায়গা সংশোধন করতে চাইতাম (অথবা আপডেট)? কেবলমাত্র আমরা সেই মানটি সংরক্ষন করবো যেটা  ফাংশন  ভেরিয়াবেল `sentence`  মাধ্যমে ফেরত পাঠিয়েছেঃ

```
    var sentence = "time for a nap"
    sentence = makeMoreExciting(sentence)
```


এখন `sentence` এর  মধ্যে বিস্ময়বোধক চিহ্ন থাকবে! মনে রাখবে তুমি শুধুমাত্র  তখনি  `var`  ব্যবহার করতে পারবে যখন ভেরিয়াবেল আরম্ভ করবে প্রথমবারের মত । এর পরে আপনি `var` ব্যবহার না করা উচিত যদি না আপনি পুনরায় ভেরিয়াবেল  আরম্ভ (পুনরায় সেট / পরিষ্কার / খালি)  করতে চান।

  কি হতে পারে যদি আমরা `return`  স্টেটমেন্ট ফাংশন থেকে বাদ দিয়ে দেই?

 ![console](images/custom-function-no-return.gif)


  `sentence`  টি ফাঁকা কেন? কারণ ফাংশন   `undefined` ফেরত পাঠায় ডিফল্ট দ্বারা !   আপনি নির্বাচন  করতে পারবেন একটি  ফেরতকৃত মান কোনোকিছু ফেরত দিয়ে । ফাংশনগুলির একটি মান গ্রহণ করা উচিত এবং, যদি তারা মান পরিবর্তন করে বা একটি নতুন মান তৈরি করে যা পরে ব্যবহার করা অনুমিত হয়, একটি  মান ফেরত (মজার বিষয় হল: এই শৈলীর জন্য একটি অভিনব শব্দ ফাংশনাল প্রোগ্রামিং)। এখানে অন্য একটি ফাংশন রয়েছে যা কিছু ফেরৎ দেয় না কিন্তু এর পরিবর্তে আমাদের আউটপুট প্রদর্শন করে একটি ভিন্ন পদ্ধতি ব্যাবহারের মাধ্যমে:

```js
function yellIt(string) {
  string = string.toUpperCase()
  string = makeMoreExciting(string)
  console.log(string)
}
```

এই ফাংশন, `yellIt`, আমাদের পূর্বের ফাংশনটি  `makeMoreExciting` ব্যবহার করে  উপরন্তু,  স্ট্রিং মেথড  toUpperCase  তৈরি করে।
মেথডস একটি নাম ফাংশন এর জন্য যখন এটি কিছুর সাথে সম্পর্কিত - এই ক্ষেত্রে `toUpperCase` একটি ফাংশন যা স্ট্রিং এর সাথে সম্পর্কিত তাই আমরা এটিকে পদ্ধতি বা একটি ফাংশন হিসাবে উল্লেখ করতে পারি। অন্যদিকে `makeMoreExciting` কোনকিছুর সাথে সম্পর্কিত নয় তাই  এটি টেকনিক্যালি ভুল হবে যদি এটাকে মেথড হিসেবে উল্লেখ করা হয়( বিভ্রান্তিকর, আমি জানি)। 

 ফাংশনের শেষ লাইনটি আরেকটু অন্তর্নির্মিত- যেটিতে তুমি কেবল যে কোনও মান দিয়ে দিবে এবং প্রিন্ট করে দিবে কনসোলে । 

 ![console](images/custom-function-console-log.gif)

  উপরের `YellIt`  ফাংশনের সঙ্গে কিছু ভুল আছে? এটা নির্ভর করে! এখানে দুটি প্রধান ফাংশন রয়েছেঃ 

*  ফাংশন যা পরিবর্তন করে বা মান তৈরি করে এবং তাদের ফেরত দেয়।
*  ফাংশন মান গ্রহণ করে এবং কিছু কর্ম সঞ্চালিত করে যা ফেরত পাওয়া যাবে না ।


   `console.log` হল দ্বিতীয় ধরনের ফাংশনের একটি উদাহরণ: এটি  তোমার  কাজকে প্রিন্ট করে দেয় কনসোলে - এমন একটি কাজ  যা তুমি তোমার চোখ দিয়ে  দেখতে পারো কিন্তু এটি জাভাস্ক্রিপ্ট মান হিসাবে উপস্থাপন করা যায় না । আমার নিজস্ব নিয়ম হল দুই ধরনের ফাংশনকে একে অপরের থেকে আলাদা রাখার চেষ্টা করা, তাই এখানে আমি `yellIt` ফাংশনটি পুনর্লিখন করব যেভাবেঃ

```js
function yellIt(string) {
  string = string.toUpperCase()
  return makeMoreExciting(string)
}

console.log(yellIt("i fear no human"))
```


এইভাবে `yellIt` আরও জাতিবাচক হয়ে যায়, যার অর্থ এটি কেবল একটি বা দুইটি সাধারণ ছোট্ট জিনিসগুলি করে এবং নিজেকে একটি কনসোলের মুদ্রণ সম্পর্কে কিছুই জানে না - যে অংশটি পরে ফাংশনের সংজ্ঞা ছাড়াই প্রোগ্রাম করা যায়। 


### <a id="loops" href="#loops">#</a> Loops

এখন যেহেতু আমাদের কিছু সাধারণ দক্ষতা আছে(লেখকের নোট: বিড়ালও বেল্ট পরে?) আমরা আলসামি করতে পারি। কি?! হ্যা, এইটাই ঠিক: প্রোগ্রামিং হচ্ছে আলসামি। ল্যারি ওয়াল, Perl প্রোগ্রামিং ল্যাঙ্গুয়েজের আবিষ্কারক বলেছেন আলসামি হচ্ছে একজন ভালো প্রোগ্রামারের সবচেয়ে ভালো গুন।  যদি কম্পিউটার না থাকতো তাহলে সব রকমের ক্লান্তিকর কঠিন কাজ গুলো তোমাকরে নিজ হাতে করতে হতো। কিন্তু তুমি যদি প্রোগ্রামিং পারো তাহলে তুমি সারাদিন সূর্যের নাইস থাকতে পারবে আর তোমার কম্পিউটার স্বয়ংক্রিয়ভাবে তোমার করা প্রোগ্রামগুলো চালিয়ে যাবে । এটি একটি গৌরবময় জীবনধারা বিশ্রাম সঙ্গে ভরা! 

লুপ হলো একটি কম্পিউটারের শক্তি ব্যবহার করার সবচেয়ে গুরুত্বপূর্ণ উপায়। ```Underscore.js```  এর কথা মনে আছে?
নিশ্চিত করো ফাইলটি তুমি পেইজে লোড করেছো কিনা (মনে কর: তুমি শুধুমাত্র তোমার কি-বোর্র্ডের up-Arrow  কয়েকবার চেপে Enter  এ চাপ দিলেই ফাইলটি লোড হয়ে যাবে) এবং সেটিকে তোমার কনসোলে  কপি/পেস্ট করো:
```
function logANumber(someNumber) {
  console.log(someNumber)
}
_.times(10, logANumber)
```

এই কোডটি Underscore  এর  [time](http://underscorejs.org/#times)  মেথড টি প্রদর্র্শন করে যেটা একটি সংখ্যা নেয় এবং একটি ফাংশন তারপর এটি ০ থেকে ১০ পর্যন্ত গণনা করে।

![console](https://github.com/entrptaher/a-cats-guide-for-js-in-bangla/raw/master/images/times-loop.png "console")

যদি আমরা একই ফলাফল পেতে চাই তাহলে আমরা কোডটি এইভাবে লিখতাম: 
```
logANumber(0)
logANumber(1)
logANumber(2)
logANumber(3)
logANumber(4)
logANumber(5)
logANumber(6)
logANumber(7)
logANumber(8)
logANumber(9)
```

কিন্তু বিড়াল কখনও অপ্রয়োজনীয় কাজ করে না তাই আমরা আমাদের কে সবসময় জিজ্ঞাসা করবো " আমি কি এইটা কোনো অলস উপায়ে করছি?" 

তো কেন এটিকে  লুপিং  বলা হয়? এইভাবে চিন্তা করো: যদি আমাদেরকে জাভাস্ক্রিপ্ট 
অ্যারে ব্যবহার করে ১০টি সংখ্যার একটি লিস্ট লিখতে দেয়া হয় (০ থেকে 9)  তাহলে এটি এরকম দেখাবে:
‍‍‍‍‍‍```var zeroThroughTen = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]‍‍‍
```

 ```time``` মেথডটি এই অ্যারের প্রত্যেকটি উপাদানে একবার করে যায় এবং সংখ্যাটি ফেরত পাঠায়। উপরের উদাহরণে 
কাজটির নাম দেয়া হয়েছে ```logNumber``` যেটা  নাম্বারগুলোকে লগ করবে।
এভাবে কাজগুলিকে পুনরাবৃত্তি করা হয় অ্যারের উপর *লুপিং* করে।

### <a id="arrays" href="#arrays">#</a> Arrays

আমি আগেই অ্যারে কয়েকবার ব্যবহার করেছি কিন্তু আসো এইবার কিছু সময় কাটাই অ্যারে শিখতে। কল্পনা কর তোমার  সব বন্ধুদেরকে তুমি একটি লিস্টে রাখবে। অ্যারে এইখানে ব্যবহার করা যেতে পারে । চিন্তা কর একটা অ্যারে যেখানে তুমি তুমি হাজার হাজার ড্যাটা সংরক্ষণ করতে পারবে।
এইভাবে তুমি একটি অ্যারে বানাতে পারো:
```
var myCatFriends = ["bill", "tabby", "ceiling"]
```
সেই! এখন তোমার কাছে তোমার বিড়াল বন্ধুদের একটি লিস্ট আছে।
উপাদান(যাকে তুমি এই অ্যারের উপাদান বলতে পারো) যেগুলো তোমার অ্যারেতে সংরক্ষিত আছে সেগুলো ০ থেকে শুরু হবে এবং এক এক করে বাড়বে। অতএব ```myCatFriends[0]``` 'bill' কে ফলাফল হিসেবে বের করবে এবং ```myCatFriends[1]```  'tabby' কে ইত্যাদি ইত্যাদি।
লিস্ট হতে তোমার বন্ধুদের নাম সরাসরি বের করতে এই কোডটি লেখো :
```
console.log(myCatFriends[0])
```
![console](https://github.com/entrptaher/a-cats-guide-for-js-in-bangla/raw/master/images/array-access.png "console")

এখন তুমি যদি তোমার এই বিড়াল বন্ধুদের লিস্টে নতুন কোনো বন্ধুকে এড করতে কেও তাহলে তাহলে এই রুলটি ফল করো:

```myCatFriends.push("super hip cat")```

নতুন বন্ধুটি যুক্ত হয়েছে কিনা তা বের করতে ‍‍‍```.length```  ব্যবহার করো।

![console](https://github.com/entrptaher/a-cats-guide-for-js-in-bangla/raw/master/images/array-push-length.png "console")

লক্ষ্য করো ```push```  কিভাবে তোমার লিস্টের  দৈর্ঘ্য রিটার্র্ন করলো. সেই!  এবং মনে রাখো তুমি যেই সিরিয়ালে ড্যাটা রাখবে অ্যারে সেই সিরিয়ালই প্রদর্র্শন করবে। জাভাস্ক্রিপ্টে সব কিছু সিরিয়াল মনে রাখে না।এটাই হলো অ্যারের বিশেষ দিক!


### <a id="objects" href="#objects">#</a> Objects

লিস্টের জন্য অ্যারে ভালো তবে কিছু ক্ষেত্রে তা ব্যবহার করা কঠিন হয়ে যায়।এখন কি হবে যদি তুমি নাম ছাড়া আরো কিছু এড করতে চাও? 
```
var myCatFriends = ["bill", "tabby", "ceiling"]
var lastNames = ["the cat", "cat", "cat"]
var addresses = ["The Alley", "Grandmas House", "Attic"]
```
কিছু ক্ষেত্রে সব নাম অথবা সব ঠিকানা একটি ভেরিয়েবল রাখা ভালো। কিন্তু কিছু সময় তুমি শুধু মাত্র একটি বিড়ালের কথা চিন্তা করবে। মনে করো  Bill,  আর তুমি শুধু তারই ঠিকানা দেখতে চাও। অ্যারের ক্ষেত্রে তোমাকে এইখানে অনেক কাজ করতে হবে। কারণ তুমি অ্যারেকে বলতে পারবে না "হেই অ্যারে,আমাকে  Bill  এর ঠিকানা দাও "। কারণ  "Bill"  একটি অ্যারেতে আর তার ঠিকানা আরেকটি অ্যারেতে। 

![console](https://github.com/entrptaher/a-cats-guide-for-js-in-bangla/raw/master/images/array-lookup.png "console")

এটি ভেঙ্গে জিতে পারে।কারণ যদি আমাদের অ্যারেগুলো পরিবর্তিত হয় এবং আমরা যদি নতুন কোনো বিড়াল তাতে এড করি তাহলে আমাদের কে ```billsPosition``` ও আপডেট করতে হবে Bill  এর তথ্য অ্যারেতে পাওয়ার জন্য।
object  এর মাধ্যমে আরো সহজে তথ্য গুলো সংরক্ষণ করা যায়:
```
var firstCat = { name: "bill", lastName: "the cat", address: "The Alley" }
var secondCat = { name: "tabby", lastName: "cat", address: "Grandmas House" }
var thirdCat = { name: "ceiling", lastName: "cat", address: "Attic" }
```

কেন আমরা এই পদ্ধতি ব্যবহার করবো? কারণ, এখন আমাদের কাছে একটি ভেরিয়েবল আছে যেখানে একটি বিড়ালের যাবতীয় তথ্য গুলো সংরক্ষিত আছে যে খুব সহজেই বুঝা ও পড়া যায় ।

![console](https://github.com/entrptaher/a-cats-guide-for-js-in-bangla/raw/master/images/object-lookup.png "console")

তুমি মনে করতে পারো অবজেক্ট হলো চাবির মতো যে চাবির  গোছায় আটকানো। একেকটি চাবি একটি দরজার জন্য এবং যদি তোমার কাছে সজ্জিত চাবির গোছা থাকে তাহলে তুমি সহজেই দরজা খুলতে পারবে।  আসলে বাম পাশে যে ‍‍‍```:``` আছে সেটাকে বলা হয় **keys** (এদেরকে **properties** বলা হয় ) এবং ডান পাশের গুলোকে বলা হয় **value**। 
```
// এখানে key  হচ্ছে  name  আর  value  হচ্ছে  "bill"
{ name: 'bill' }
```

অতএব কেন আমরা অ্যারে ব্যবহার করবো যেখানে আমরা অব্জেক্টেই ডাটা রাখতে পারি? কারণ, অবজেক্ট তোমার দেয়া দাতার সিরিয়াল মনে রাখতে পারে না।
তুমিয এইভাবে কিছু ডাটা রাখতে পারো: 
```
{ date: "10/20/2012", diary: "slept a bit today", name: "Charles" }
```
কিন্তু কম্পিউটার তোমাকে ব্যাক করবে এইভাবে: 
```
{ diary: "slept a bit today", name: "Charles", date: "10/20/2012" }
```
অথবা এইভাবে: 
```
{ name: "Charles", diary: "slept a bit today", date: "10/20/2012" }
```
সুতরাং তুমি তোমার অবজেক্ট এর  **keys**  কে বিশ্বাস নাও করতে পারো।
তুমি যদি এই সমস্যায় পরে যাও তাহলে তুমি একটি অ্যারে তৈরী করতে পারো যাতে থাকবে অবজেক্ট অথবা একটি অবজেক্ট যাতে থাকবে অ্যারে।
```
var moodLog = [
  {
    date: "10/20/2012",
    mood: "catnipped"
  },
  {
    date: "10/21/2012",
    mood: "nonplussed"
  },
  {
    date: "10/22/2012",
    mood: "purring"
  }
]

// ordered from least to most favorite
var favorites = {
  treats: ["bird sighting", "belly rub", "catnip"],
  napSpots: ["couch", "planter box", "human face"]
}
```
এইভাবে যখন তুমি বিভিন্ন জিনিস একত্রে রাখতে কেও তুমি এই ডাটার ধরণ ব্যবহার করতে পারো!


### <a id="callbacks" href="#callbacks">#</a> Callbacks

Callbacks aren't really a feature of JavaScript like `Object` or `Array`, but instead just a certain way to use functions. To understand why callbacks are useful you first have to learn about asynchronous (often shortened to async) programming. Asynchronous code by definition is code written in a way that is not synchronous. Synchronous code is easy to understand and write. Here is an example to illustrate:

```js
var photo = download('http://foo-chan.com/images/sp.jpg')
uploadPhotoTweet(photo, '@maxogden')
```

This synchronous [pseudo-code](http://simple.wikipedia.org/wiki/Pseudocode) downloads an adorable cat photo and then uploads the photo to twitter and tweets the photo at `@maxogden`. Pretty straightforward!

(*Author's note: I @maxogden do happily accept random cat photo tweets*)

This code is synchronous because in order for photo to get uploaded to the tweet, the photo download must be completed. This means that line 2 cannot run until the task on line 1 is totally finished. If we were to actually implement this pseudo-code we would want to make sure that `download` 'blocked' execution until the download was finished, meaning it would prevent *any* other JavaScript from being executed until it finished, and then when the download completes it would un-block the JavaScript execution and line 2 would execute.

Synchronous code is fine for things that happen fast, but it's horrible for things that require saving, loading, downloading or uploading. What if the server you're downloading the photo from is slow, or the internet connection you are using is slow, or the computer you are running the code on has too many youtube cat video tabs open and is running slowly? It means that it could potentially take minutes of waiting before line 2 gets around to running. Meanwhile, because all JavaScript on the page is being blocked from being run while the download is happening, the webpage would totally freeze up and become unresponsive until the download is done.

Blocking execution should be avoided at all costs, especially when doing so makes your program freeze up or become unresponsive. Let's assume the photo above takes one second to download. To illustrate how long one second is to a modern computer, here is a program that tests to see how many tasks JavaScript can process in one second.

```js
function measureLoopSpeed() {
  var count = 0
  function addOne() { count = count + 1 }

  // Date.now() returns a big number representing the number of
  // milliseconds that have elapsed since Jan 01 1970
  var now = Date.now()

  // Loop until Date.now() is 1000 milliseconds (1 second) or more into
  // the future from when we started looping. On each loop, call addOne
  while (Date.now() - now < 1000) addOne()

  // Finally it has been >= 1000ms, so let's print out our total count
  console.log(count)
}

measureLoopSpeed()
```

Copy-paste the above code into your JavaScript console and after one second it should print out a number. On my computer I got `8527360`, approximately **8.5 million**. In one second JavaScript can call the `addOne` function 8.5 million times! So if you have synchronous code for downloading a photo, and the photo download takes one second, it means you are potentially preventing 8.5 million operations from happening while JavaScript execution is blocked.

Some languages have a function called `sleep` that blocks execution for some number of seconds. For example here is some [`bash`](http://en.wikipedia.org/wiki/Bash_%28Unix_shell%29) code running in `Terminal.app` on Mac OS that uses `sleep`. When you run the command `sleep 3 && echo 'done sleeping now'` it blocks for 3 seconds before printing out `done sleeping now`.

![console](images/bash-sleep.png)

JavaScript doesn't have a `sleep` function. Since you are a cat you are probably asking yourself, "Why am I learning a programming language that does not involve sleeping?". But stay with me. Instead of relying on `sleep` to wait for things to happen the design of JavaScript encourages use of functions instead. If you have to wait for task A to finish before doing task B, you put all of the code for task B into a function and you only call that function when A is done.

For example, this is blocking-style code:

```js
a()
b()
```

And this is in a non-blocking style:

```js
a(b)
```

In the non-blocking version `b` is a callback to `a`. In the blocking version `a` and `b` are both called/invoked (they both have `()` after them which executes the functions immediately). In the non-blocking version you will notice that only `a` gets invoked, and `b` is simply passed in to `a` as an argument.

In the blocking version, there is no explicit relationship between `a` and `b`. In the non-blocking version it becomes `a`'s job to do what it needs to do and then call `b` when it is done. Using functions in this way is called callbacks because your callback function, in this case `b`, gets called later on when `a` is all done.

Here is a pseudocode implementation of what `a` might look like:

```js
function a(done) {
  download('https://pbs.twimg.com/media/B4DDWBrCEAA8u4O.jpg:large', function doneDownloading(error, png) {
    // handle error if there was one
    if (err) console.log('uh-oh!', error)

    // call done when you are all done
    done()
  })
}
```

Think back to our non-blocking example, `a(b)`, where we call `a` and pass in `b` as the first argument. In the function definition for `a` above the `done` argument *is* our `b` function that we pass in. This behavior is something that is hard to wrap your head around at first. When you call a function, the arguments you pass in won't have the same variable names when they are in the function. In this case what we call `b` is called `done` inside the function. But `b` and `done` are just variable names that point to the same underlying function. Usually callback functions are labelled something like `done` or `callback` to make it clear that they are functions that should be called when the current function is done.

So, as long as `a` does it's job and called `b` when it is done, both `a` and `b` get called in both the non-blocking and blocking versions. The difference is that in the non-blocking version we don't have to halt execution of JavaScript. In general non-blocking style is where you write every function so that it can return as soon as possible, without ever blocking.

To drive the point home even further: If `a` takes one second to complete, and you use the blocking version, it means you can only do one thing. If you use the non-blocking version (aka use callbacks) you can do *literally millions* of other things in that same second, which means you can finish your work millions of times faster and sleep the rest of the day.

Remember: programming is all about laziness and you should be the one sleeping, not your computer.

Hopefully you can see now that callbacks are just functions that call other functions after some asynchronous task. Common examples of asynchronous tasks are things like reading a photo, downloading a song, uploading a picture, talking to a database, waiting for a user to hit a key or click on someone, etc. Anything that takes time. JavaScript is really great at handling asynchronous tasks like these as long as you take the time to learn how to use callbacks and keep your JavaScript from being blocked.

## The end!

This is just the beginning of your relationship with JavaScript! You can't learn it all at once, but you should find what works for you and try to learn all of the concepts here.

I'd recommend coming back again tomorrow and going through the entire thing again from the beginning! It might take a few times through before you get everything (programming is hard). Just try to avoid reading this page in any rooms that contain shiny objects . . . they can be incredibly distracting.

Got another topic you wanna see covered? Open an issue for it [on github](http://github.com/maxogden/javascript-for-cats).

### <a id="recommended-reading" href="#recommended-reading">#</a> Recommended reading

  JavaScript For Cats skips over lots of details that aren't important for getting started (cats are not known for their attention spans), but if you feel like you need to dive in deeper then check these out:

  - [NodeSchool.io](http://nodeschool.io/) is a community driven, open source educational software that teaches various web development skills in an interactive, self-guided format. I helped make NodeSchool! Sadly it features fewer cats than this page.
  - [Eloquent Javascript](http://eloquentjavascript.net/) is a free book that teaches you JavaScript! It's pretty good! Especially the chapter on [values, variables, and control flow](http://eloquentjavascript.net/chapter2.html)
  - [Mozilla's JavaScript Guide](https://developer.mozilla.org/en-US/docs/JavaScript/Guide) also has a pretty sweet intro chapter called [values, variables and literals](https://developer.mozilla.org/en-US/docs/JavaScript/Guide/Values,_variables,_and_literals)
  - [`standard` JS Style Guide](https://github.com/feross/standard) is a "zero configuration" linter for JS style that I use
  - [Let's Write Code by @shama](https://github.com/shama/letswritecode) a great series of YouTube coding tutorials made by a friend of mine

<hr>
### <a id="satisfied-customers" href="#satisfied-customers">#</a> Satisfied customers
<center>![satisfied customer](images/customers5.jpg)</center>
<center>![satisfied customer](images/customers1.png)</center>
<center>![satisfied customer](images/customers2.png)</center>
<center>![satisfied customer](images/customers3.png)</center>
<center>![satisfied customer](images/customers4.png)</center>

# ক্রেডিটঃ
- [Maxwell Ogden](https://twitter.com/denormalize) এর [JavaScript For Cats](https://github.com/maxogden/javascript-for-cats) হতে প্রত্যক্ষভাবে অনুপ্রাণিত।
