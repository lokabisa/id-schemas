# Place Schema

`place` adalah schema komposit yang merepresentasikan satu entitas tempat
dengan lokasi fisik dan informasi operasional minimum.

Schema ini disusun dari schema dasar Lokabisa seperti address, geo,
hours, status, dan contact, menggunakan pendekatan komposisi (`$ref`).

Schema ini dirancang agar tetap valid meskipun data yang tersedia bersifat parsial.
