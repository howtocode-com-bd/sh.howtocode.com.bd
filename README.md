<iframe src="https://www.facebook.com/plugins/likebox.php?href=https%3A%2F%2Fwww.facebook.com%2Fhowtocode.com.bd&amp;width&amp;height=62&amp;colorscheme=light&amp;show_faces=false&amp;header=false&amp;stream=false&amp;show_border=false&amp;appId=353725671441956" scrolling="no" frameborder="0" style="border:none; overflow:hidden; height:62px; margin-left:-15px;" allowTransparency="true"></iframe>

[কোর্স এর মুল পাতা](http://sh.howtocode.com.bd/) | [HowToCode মূল সাইট](http://www.howtocode.com.bd/) | [সবার জন্য প্রোগ্রামিং ব্লগ](http://blog.howtocode.com.bd/) | [পিডিএফ ডাউনলোড](https://www.gitbook.com/download/pdf/book/howtocode-com-bd/-sh)

# শেল ও শেলস্ক্রিপ্টিং

<iframe scrolling="auto" frameborder="0" style="border:none; overflow:hidden; height:170px; width:100%; margin-left: 15;" allowTransparency="true" src="http://api.howtocode.com.bd/contrib/sh"></iframe>


#### সংক্ষেপ

লিনাক্স শেল এবং শেলস্ক্রপ্টিং এর প্রাথমিক পাঠ এটি। একটি ওপেনসোর্স প্রোজেক্ট বলে আশা করা যাচ্ছে বাঙলায় লিনাক্স শেল এর সকল খুঁটিনাটি ক্রমে যুক্ত হবে।

#### ওপেন সোর্স

এই বইটি মূলত স্বেচ্ছাশ্রমে লেখা এবং বইটি সম্পূর্ন ওপেন সোর্স । এখানে তাই আপনিও অবদান রাখতে পারেন লেখক হিসেবে । আপনার কন্ট্রিবিউশান গৃহীত হলে অবদানকারীদের তালিকায় আপনার নাম যোগ করে দেওয়া হবে ।

এটি মূলত একটি [গিটহাব রিপোজিটোরি](https://github.com/howtocode-com-bd/sh.howtocode.com.bd) যেখানে এই বইয়ের আর্টিকেল গুলো মার্কডাউন ফরম্যাটে লেখা হচ্ছে। রিপোজটরিটি ফর্ক করে পুল রিকুয়েস্ট পাঠানোর মাধ্যমে আপনারাও অবদান রাখতে পারেন ।


# শুরুর কথা #

গ্রাফিলক্যাল কম্পিউটিং এর দুনিয়ায় কমান্ডলাইন শিখতে যাওয়া প্রাথমিকভাবে হাস্যকর মনে হতে পারে। এটা সত্যি আপনি কমান্ডলাইনে ফেসবুক ব্যবহার করতে পারবেন না। ভিডিও দেখতে পারবেন না দেখার মতই এবং গ্রাফিক্স ডিজাইনও সম্ভব হবে না সহজে।

কিন্তু, লিনাক্স কমান্ডলাইন বা টার্মিনাল শেখাটা আপনার লিনাক্স ব্যবহারের অভিজ্ঞতার কিছু স্থায়ী পরিবর্তন আনবে। সম্ভবত প্রথমবার আপনি বুঝতে পারবেন পাওয়ার ইউজার হওয়ার আসল অর্থটি কি।

আসুন, আপনাকে এর ক্ষমতার একটা ছোট উদাহরণ দিই। একবার আমার ২শতাধিক ছোট ছোট লেখা মাইক্রোসফট ওয়ার্ড ডকুমেন্ট থেকে প্লেইন টেক্সটে কনভার্ট করার দরকার পড়েছিল। আমি হয়ত প্রত্যেকটা ফাইল খুলে সেখান থেকে টেক্সট ফরম্যাটে সেভ দিতে পারতাম। কিন্তু টার্মিনালে মাত্র একটি কমান্ডের মাধ্যমে আমি মাত্র কয়েকসেকেন্ডে সবগুলো ফাইল কনভার্ট করেছি।

## আপনার যা যা প্রয়োজন হবে: ##

এই কোর্সটি কম্প্লিট করতে আপনার একটি লিনাক্সভিত্তিক অপারেটিং সিস্টেম প্রয়োজন হবে। আমি এটা লেখা শুরুর সময়ে উবুন্টু জিনোম ১৪.০৪ ব্যবহার করেছি।

**কোনো কোনো ক্ষেত্রে আমি টার্মিনালেই সরাসরি বাঙলা ব্যবহার করেছি। এটা জরুরি কিছুই নয়। অনেক টার্মিনাল ইমুলেটরের বাঙলা ফন্ট রেন্ডারিং হতাশাজনক। তবে আপনি চাইলে konsole ও konsoleনির্ভর ড্রপডাউন টার্মিনাল ইমুলেটর ব্যবহার করতে পারেন।

## কৃতজ্ঞতা ##

উইলিয়াম শটস জুনিয়র('দি লিনাক্স কমান্ডলাইন' বইটির লেখক)

তাহলে আসুন, শুরু করা যাক!

<iframe src="https://www.facebook.com/plugins/like.php?href=http%3A%2F%2Fsh.howtocode.com.bd&amp;width&amp;layout=button_count&amp;action=like&amp;show_faces=false&amp;share=true&amp;height=21&amp;appId=353725671441956" scrolling="no" frameborder="0" style="border:none; overflow:hidden; height:21px;" allowTransparency="true"></iframe>
