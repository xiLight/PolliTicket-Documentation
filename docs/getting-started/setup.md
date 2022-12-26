# How to setup

⚡️ Every single step is explained in detail and the difference between quick and normal setup is explained.

---

## Quick setup

**Command:** /Quicksetup<br>
**Permission:** ADMINISTRATOR

Only 2 arguments are required for Quicksetup.
The [**setup name**](#) and a [**language**](#).
This command is meant to test quickly and easily.

You can easily edit your setup in the web panel and adapt it to your needs.
For the webpanel it is necessary to be on our Discord.

Since the quick command only requires 2 arguments, the rest is filled in automatically by us.

**Required**

- `setup-name`
- `language`

**Defaults**

- `timezone` UTC
- `use-transcripts` false ( Offline Archive )
- `log-channel` 📛・transcripts-log ( Automatically created )
- `tickets-spacer-name` 🎫| **setup-name** Tickets |🎫 ( Automatically created )
- `create-channel` 🎫・general-ticket ( Automatically created )
- `team-role` **setup-name** team ( Automatically created )
- `ping-role` is team-role
- `max-tickets-per-user` 1
- `response-within-label` 24 hours
- `auto-close-time` 3d
- `custom-text` EditMe in our panel
- `embed-image-url` null

---

## Normal setup

**Command:** /Setup<br>
**Permission:** ADMINISTRATOR

Unlike quicksetup, all required arguments must be filled in here.
We explain all the arguments here so that you can get through all the steps.

---

### Steps before Setup

In order to be able to make the setup, you need a few small things in advance:

!!! note

    If there is already a role for the team to see and edit tickets, then you can jump to the second point.

- Create **1** or **2** new roles (Ping and Team role) for your team.<br>
  You can also create only 1 role, for example `team`, which you can use to ping and edit tickets. It is important that **at least one role** is available.

!!! note

    If a TextChannel already exists where tickets can be created, you can also use this TextChannel in the setup, simply select your TextChannel in the setup under `Create-Channel`.

- Create a TextChannel, where the TicketCreator ( Embed ) will land after the setup, new tickets can be created in this TextChannel by clicking on the button.

!!! note

    If there is already a TextChannel where you store logs, you can select this TextChannel in the setup under `Log-Channel`.

- Create a TextChannel where Bot can post the transcript logs after closing tickets. Please make sure that the bot can write/read there and post embeds.
- If you already have a category where tickets end up, you can copy the category name and paste it into the setup under `Tickets-spacer-name`. <br>If this category does not exist, a new category with this name will be created.
- Check our [required permissions](../permissions/bot-permissions.md)

---

### Checklist

**Info**

- [x] Important, to use the bot.
- [ ] Not mandatory.

---

- [x] Checked whether the bot has all the permissions required to
    1. Create channels, categories and roles.
    2. Must be able to send embeds/messages in the log, ticket and creator channel.
- [x] Read through all steps [before setup](#)
- [ ] Joined our [Discord](https://discord.polliticket.eu) to use our panel.

---

### Setup-Name

Here you have to think of a name for your setup, this name is in the panel under settings after the setup and is used in the quicksetup to create the roles and categories.

---

### Timezone

Here you have to enter a timezone so that the bot knows how to handle your time.
Because there are many timezones, I have listed the most common timezones.

`Most common timezones:` UTC, Europe/Berlin

??? note "Timezone list"

    ACT,AET,AGT,ART,AST,Africa/Abidjan,Africa/Accra,Africa/Addis_Ababa,Africa/Algiers,Africa/Asmara,Africa/Asmera,Africa/Bamako,Africa/Bangui,Africa/Banjul,Africa/Bissau,Africa/Blantyre,Africa/Brazzaville,Africa/Bujumbura,Africa/Cairo,Africa/Casablanca,Africa/Ceuta,Africa/Conakry,Africa/Dakar,Africa/Dar_es_Salaam,Africa/Djibouti,Africa/Douala,Africa/El_Aaiun,Africa/Freetown,Africa/Gaborone,Africa/Harare,Africa/Johannesburg,Africa/Juba,Africa/Kampala,Africa/Khartoum,Africa/Kigali,Africa/Kinshasa,Africa/Lagos,Africa/Libreville,Africa/Lome,Africa/Luanda,Africa/Lubumbashi,Africa/Lusaka,Africa/Malabo,Africa/Maputo,Africa/Maseru,Africa/Mbabane,Africa/Mogadishu,Africa/Monrovia,Africa/Nairobi,Africa/Ndjamena,Africa/Niamey,Africa/Nouakchott,Africa/Ouagadougou,Africa/Porto-Novo,Africa/Sao_Tome,Africa/Timbuktu,Africa/Tripoli,Africa/Tunis,Africa/Windhoek,America/Adak,America/Anchorage,America/Anguilla,America/Antigua,America/Araguaina,America/Argentina/Buenos_Aires,America/Argentina/Catamarca,America/Argentina/ComodRivadavia,America/Argentina/Cordoba,America/Argentina/Jujuy,America/Argentina/La_Rioja,America/Argentina/Mendoza,America/Argentina/Rio_Gallegos,America/Argentina/Salta,America/Argentina/San_Juan,America/Argentina/San_Luis,America/Argentina/Tucuman,America/Argentina/Ushuaia,America/Aruba,America/Asuncion,America/Atikokan,America/Atka,America/Bahia,America/Bahia_Banderas,America/Barbados,America/Belem,America/Belize,America/Blanc-Sablon,America/Boa_Vista,America/Bogota,America/Boise,America/Buenos_Aires,America/Cambridge_Bay,America/Campo_Grande,America/Cancun,America/Caracas,America/Catamarca,America/Cayenne,America/Cayman,America/Chicago,America/Chihuahua,America/Coral_Harbour,America/Cordoba,America/Costa_Rica,America/Creston,America/Cuiaba,America/Curacao,America/Danmarkshavn,America/Dawson,America/Dawson_Creek,America/Denver,America/Detroit,America/Dominica,America/Edmonton,America/Eirunepe,America/El_Salvador,America/Ensenada,America/Fort_Wayne,America/Fortaleza,America/Glace_Bay,America/Godthab,America/Goose_Bay,America/Grand_Turk,America/Grenada,America/Guadeloupe,America/Guatemala,America/Guayaquil,America/Guyana,America/Halifax,America/Havana,America/Hermosillo,America/Indiana/Indianapolis,America/Indiana/Knox,America/Indiana/Marengo,America/Indiana/Petersburg,America/Indiana/Tell_City,America/Indiana/Vevay,America/Indiana/Vincennes,America/Indiana/Winamac,America/Indianapolis,America/Inuvik,America/Iqaluit,America/Jamaica,America/Jujuy,America/Juneau,America/Kentucky/Louisville,America/Kentucky/Monticello,America/Knox_IN,America/Kralendijk,America/La_Paz,America/Lima,America/Los_Angeles,America/Louisville,America/Lower_Princes,America/Maceio,America/Managua,America/Manaus,America/Marigot,America/Martinique,America/Matamoros,America/Mazatlan,America/Mendoza,America/Menominee,America/Merida,America/Metlakatla,America/Mexico_City,America/Miquelon,America/Moncton,America/Monterrey,America/Montevideo,America/Montreal,America/Montserrat,America/Nassau,America/New_York,America/Nipigon,America/Nome,America/Noronha,America/North_Dakota/Beulah,America/North_Dakota/Center,America/North_Dakota/New_Salem,America/Ojinaga,America/Panama,America/Pangnirtung,America/Paramaribo,America/Phoenix,America/Port-au-Prince,America/Port_of_Spain,America/Porto_Acre,America/Porto_Velho,America/Puerto_Rico,America/Rainy_River,America/Rankin_Inlet,America/Recife,America/Regina,America/Resolute,America/Rio_Branco,America/Rosario,America/Santa_Isabel,America/Santarem,America/Santiago,America/Santo_Domingo,America/Sao_Paulo,America/Scoresbysund,America/Shiprock,America/Sitka,America/St_Barthelemy,America/St_Johns,America/St_Kitts,America/St_Lucia,America/St_Thomas,America/St_Vincent,America/Swift_Current,America/Tegucigalpa,America/Thule,America/Thunder_Bay,America/Tijuana,America/Toronto,America/Tortola,America/Vancouver,America/Virgin,America/Whitehorse,America/Winnipeg,America/Yakutat,America/Yellowknife,Antarctica/Casey,Antarctica/Davis,Antarctica/DumontDUrville,Antarctica/Macquarie,Antarctica/Mawson,Antarctica/McMurdo,Antarctica/Palmer,Antarctica/Rothera,Antarctica/South_Pole,Antarctica/Syowa,Antarctica/Troll,Antarctica/Vostok,Arctic/Longyearbyen,Asia/Aden,Asia/Almaty,Asia/Amman,Asia/Anadyr,Asia/Aqtau,Asia/Aqtobe,Asia/Ashgabat,Asia/Ashkhabad,Asia/Baghdad,Asia/Bahrain,Asia/Baku,Asia/Bangkok,Asia/Beirut,Asia/Bishkek,Asia/Brunei,Asia/Calcutta,Asia/Chita,Asia/Choibalsan,Asia/Chongqing,Asia/Chungking,Asia/Colombo,Asia/Dacca,Asia/Damascus,Asia/Dhaka,Asia/Dili,Asia/Dubai,Asia/Dushanbe,Asia/Gaza,Asia/Harbin,Asia/Hebron,Asia/Ho_Chi_Minh,Asia/Hong_Kong,Asia/Hovd,Asia/Irkutsk,Asia/Istanbul,Asia/Jakarta,Asia/Jayapura,Asia/Jerusalem,Asia/Kabul,Asia/Kamchatka,Asia/Karachi,Asia/Kashgar,Asia/Kathmandu,Asia/Katmandu,Asia/Khandyga,Asia/Kolkata,Asia/Krasnoyarsk,Asia/Kuala_Lumpur,Asia/Kuching,Asia/Kuwait,Asia/Macao,Asia/Macau,Asia/Magadan,Asia/Makassar,Asia/Manila,Asia/Muscat,Asia/Nicosia,Asia/Novokuznetsk,Asia/Novosibirsk,Asia/Omsk,Asia/Oral,Asia/Phnom_Penh,Asia/Pontianak,Asia/Pyongyang,Asia/Qatar,Asia/Qyzylorda,Asia/Rangoon,Asia/Riyadh,Asia/Riyadh87,Asia/Riyadh88,Asia/Riyadh89,Asia/Saigon,Asia/Sakhalin,Asia/Samarkand,Asia/Seoul,Asia/Shanghai,Asia/Singapore,Asia/Srednekolymsk,Asia/Taipei,Asia/Tashkent,Asia/Tbilisi,Asia/Tehran,Asia/Tel_Aviv,Asia/Thimbu,Asia/Thimphu,Asia/Tokyo,Asia/Ujung_Pandang,Asia/Ulaanbaatar,Asia/Ulan_Bator,Asia/Urumqi,Asia/Ust-Nera,Asia/Vientiane,Asia/Vladivostok,Asia/Yakutsk,Asia/Yekaterinburg,Asia/Yerevan,Atlantic/Azores,Atlantic/Bermuda,Atlantic/Canary,Atlantic/Cape_Verde,Atlantic/Faeroe,Atlantic/Faroe,Atlantic/Jan_Mayen,Atlantic/Madeira,Atlantic/Reykjavik,Atlantic/South_Georgia,Atlantic/St_Helena,Atlantic/Stanley,Australia/ACT,Australia/Adelaide,Australia/Brisbane,Australia/Broken_Hill,Australia/Canberra,Australia/Currie,Australia/Darwin,Australia/Eucla,Australia/Hobart,Australia/LHI,Australia/Lindeman,Australia/Lord_Howe,Australia/Melbourne,Australia/NSW,Australia/North,Australia/Perth,Australia/Queensland,Australia/South,Australia/Sydney,Australia/Tasmania,Australia/Victoria,Australia/West,Australia/Yancowinna,BET,BST,Brazil/Acre,Brazil/DeNoronha,Brazil/East,Brazil/West,CAT,CET,CNT,CST,CST6CDT,CTT,Canada/Atlantic,Canada/Central,Canada/East-Saskatchewan,Canada/Eastern,Canada/Mountain,Canada/Newfoundland,Canada/Pacific,Canada/Saskatchewan,Canada/Yukon,Chile/Continental,Chile/EasterIsland,Cuba,EAT,ECT,EET,EST,EST5EDT,Egypt,Eire,Etc/GMT,Etc/GMT+0,Etc/GMT+1,Etc/GMT+10,Etc/GMT+11,Etc/GMT+12,Etc/GMT+2,Etc/GMT+3,Etc/GMT+4,Etc/GMT+5,Etc/GMT+6,Etc/GMT+7,Etc/GMT+8,Etc/GMT+9,Etc/GMT-0,Etc/GMT-1,Etc/GMT-10,Etc/GMT-11,Etc/GMT-12,Etc/GMT-13,Etc/GMT-14,Etc/GMT-2,Etc/GMT-3,Etc/GMT-4,Etc/GMT-5,Etc/GMT-6,Etc/GMT-7,Etc/GMT-8,Etc/GMT-9,Etc/GMT0,Etc/Greenwich,Etc/UCT,Etc/UTC,Etc/Universal,Etc/Zulu,Europe/Amsterdam,Europe/Andorra,Europe/Athens,Europe/Belfast,Europe/Belgrade,Europe/Berlin,Europe/Bratislava,Europe/Brussels,Europe/Bucharest,Europe/Budapest,Europe/Busingen,Europe/Chisinau,Europe/Copenhagen,Europe/Dublin,Europe/Gibraltar,Europe/Guernsey,Europe/Helsinki,Europe/Isle_of_Man,Europe/Istanbul,Europe/Jersey,Europe/Kaliningrad,Europe/Kiev,Europe/Lisbon,Europe/Ljubljana,Europe/London,Europe/Luxembourg,Europe/Madrid,Europe/Malta,Europe/Mariehamn,Europe/Minsk,Europe/Monaco,Europe/Moscow,Europe/Nicosia,Europe/Oslo,Europe/Paris,Europe/Podgorica,Europe/Prague,Europe/Riga,Europe/Rome,Europe/Samara,Europe/San_Marino,Europe/Sarajevo,Europe/Simferopol,Europe/Skopje,Europe/Sofia,Europe/Stockholm,Europe/Tallinn,Europe/Tirane,Europe/Tiraspol,Europe/Uzhgorod,Europe/Vaduz,Europe/Vatican,Europe/Vienna,Europe/Vilnius,Europe/Volgograd,Europe/Warsaw,Europe/Zagreb,Europe/Zaporozhye,Europe/Zurich,GB,GB-Eire,GMT,GMT0,Greenwich,HST,Hongkong,IET,IST,Iceland,Indian/Antananarivo,Indian/Chagos,Indian/Christmas,Indian/Cocos,Indian/Comoro,Indian/Kerguelen,Indian/Mahe,Indian/Maldives,Indian/Mauritius,Indian/Mayotte,Indian/Reunion,Iran,Israel,JST,Jamaica,Japan,Kwajalein,Libya,MET,MIT,MST,MST7MDT,Mexico/BajaNorte,Mexico/BajaSur,Mexico/General,Mideast/Riyadh87,Mideast/Riyadh88,Mideast/Riyadh89,NET,NST,NZ,NZ-CHAT,Navajo,PLT,PNT,PRC,PRT,PST,PST8PDT,Pacific/Apia,Pacific/Auckland,Pacific/Bougainville,Pacific/Chatham,Pacific/Chuuk,Pacific/Easter,Pacific/Efate,Pacific/Enderbury,Pacific/Fakaofo,Pacific/Fiji,Pacific/Funafuti,Pacific/Galapagos,Pacific/Gambier,Pacific/Guadalcanal,Pacific/Guam,Pacific/Honolulu,Pacific/Johnston,Pacific/Kiritimati,Pacific/Kosrae,Pacific/Kwajalein,Pacific/Majuro,Pacific/Marquesas,Pacific/Midway,Pacific/Nauru,Pacific/Niue,Pacific/Norfolk,Pacific/Noumea,Pacific/Pago_Pago,Pacific/Palau,Pacific/Pitcairn,Pacific/Pohnpei,Pacific/Ponape,Pacific/Port_Moresby,Pacific/Rarotonga,Pacific/Saipan,Pacific/Samoa,Pacific/Tahiti,Pacific/Tarawa,Pacific/Tongatapu,Pacific/Truk,Pacific/Wake,Pacific/Wallis,Pacific/Yap,Poland,Portugal,ROK,SST,Singapore,SystemV/AST4,SystemV/AST4ADT,SystemV/CST6,SystemV/CST6CDT,SystemV/EST5,SystemV/EST5EDT,SystemV/HST10,SystemV/MST7,SystemV/MST7MDT,SystemV/PST8,SystemV/PST8PDT,SystemV/YST9,SystemV/YST9YDT,Turkey,UCT,US/Alaska,US/Aleutian,US/Arizona,US/Central,US/East-Indiana,US/Eastern,US/Hawaii,US/Indiana-Starke,US/Michigan,US/Mountain,US/Pacific,US/Pacific-New,US/Samoa,UTC,Universal,VST,W-SU,WET,Zulu

---

### Use-Transcripts

PolliTicket offers you to respect your privacy and still have an archive!
A dropdown must be used to select between `true` and `false`.

- `true` A transcript is created after the ticket close and saved online.
- `false` The ticket content is **not** saved, but the ticket is moved to an archive category for 7 days that can only be seen by an admin.

---

### Log-Channel

!!! Warning

    This TextChannel must already exist, see [Steps before Setup](#steps-before-setup).


Please select a textchannel here where the bot will post the transcripts and logs.

---

### Tickets-Spacer-Name

!!! info

    If category already exists, the existing category is taken.

Think of a name for a category where new tickets end up.

---

### Create-Channel

!!! Warning

    This TextChannel must already exist, see [Steps before Setup](#steps-before-setup).

Choose a channel from dropdown where the ticket creator ends up inside.
The ticket creator is an embed message with a button. With this button you can create a new ticket as long as the MaxTickets for users is greater than 0.

---

### Team-Role

!!! Warning

    This role must already exist, see [Steps before Setup](#steps-before-setup).

A drop-down menu must be used to select the supporter role that has the right to view, close and claim a ticket.
Roles with administrator permission can see tickets even without supporter role.

---

### Ping-Role

!!! Warning

    This role must already exist, see [Steps before Setup](#steps-before-setup).

A drop-down menu must be used to select the ping role that will be pinged as soon as a new ticket has been created.

---

### Max-Tickets-Per-User:

!!! info

    If you set the maximum number in the panel to 0, no more tickets can be created. This is not a bug, but a feature.

It determines how many tickets a user may have open at the same time for this setup.
We recommend 1 ticket per user.

---

### Response-Within-Label

You need to describe how long it takes your support team to respond.
You can insert free text here, for example: `24 hours | Weekend 48 hours`.

---

### Auto-Close-Time

Here you can decide when the tickets should be closed automatically if there is no response after x days or x hours.

**Examples:**

- `8 hours:` 8h
- `1 day:` 1d
- `3 days:` 3d

We recommend 3 days `3d`.
After 3 days without a reply, one can assume that the support issue has been resolved.

---

### Embed-Image-Url

!!! info

    Please make sure that you enter the **full** link with `https://`

If you want a nice image at the bottom of the footer of the embed, you can enter a full link here.

**Allowed endings:**

- `.jpg`
- `.jpeg`
- `.gif`
- `.png`
- `.bmp`

---

### Custom-Text

If you would like to give your TicketCreator a beautiful custom text, then you have come to the right place.

You can create your own description, which will be placed under the info.
**Maximum 300 characters** allowed.
I would recommend use our panel, because it must be written in one line in slash commands.
