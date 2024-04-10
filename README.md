<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" />
    <script src="https://kit.fontawesome.com/1dc1877525.js" crossorigin="anonymous"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
    <title>Trang Web của Tôi</title>
    <style>
        body {
            font-family: Arial;
            padding: 10px;
            margin: 0;
        }

        /* CSS để tạo thanh điều hướng */
        .navbar {
            background-color: aliceblue;
            overflow: hidden;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .navbar a {
            color: black;
            text-decoration: none;
            padding: 10px;
        }

        .tieu-de {
            text-shadow: #ddd;
            font-size: larger;
            margin-right: 0%;
            margin-top: -5%;
        }

        .navbar a:hover {
            background-color: #ddd;
            color: black;
        }

        .search-container {
            text-align: center;
            padding: 20px;
        }

        /* CSS cho ô tìm kiếm */
        .search-container input[type="text"] {
            padding: 10px;

            margin-top: 8px;
            font-size: 17px;
            border: none;
        }

        /* CSS cho nút tìm kiếm */
        .search-container button {
            padding: 10px 20px;
            margin-top: 8px;
            background: #ddd;
            font-size: 17px;
            border: none;
            cursor: pointer;
        }

        .search-container button:hover {
            background: #ccc;
        }

        .navbar-logo img {
            width: 140px;
            height: auto;
        }

        h4 {
            text-align: center;
            font-size: larger;
        }

        img {
            width: 100%;
            height: 500px;
        }

        .row {
            display: flex;
            flex-wrap: wrap;
        }

        .side {
            flex-basis: 30%;
            background-color: #f1f1f1;
            padding: 20px;
        }

        .main {
            flex-basis: 70%;
            background-color: white;
            padding: 20px;
        }

        .newimg {
            background-color: #bce2c9;
            width: 100%;
            padding: 20px;
        }

        .row img {
            max-width: 100%;
            height: auto;
        }

        .side h3 {
            background-color: #333;
            color: #fff;
            padding: 9px;
            text-align: center;
        }

        .side h3:hover {
            color: #fff;
            background-color: aqua;
        }

        .main-content {
            margin-right: 20px;
        }

        /* CSS cho các sản phẩm */
        .product {
            border: 1px solid #ddd;
            padding: 10px;
            margin-bottom: 20px;
        }

        .product img {
            max-width: 50%;
            height: auto;
        }

        .product-info {
            display: flex;
        }

        .product-info img {
            margin-right: 10px;
        }

        .footer {
            background-color: #343a40;
            color: #ffffff;
            padding: 40px 0;
        }

        .chat-nav {
            position: fixed;
            left: 13px;
            background: #fff;
            border-radius: 5px;
            width: auto;
            top: 40%;
            padding: 8px 0;
            border: 1px solid #f2f2f2;
        }

        .chat-nav ul {
            list-style: none;
            padding: 5px;
            margin: 0;
        }

        .chat-nav ul li a {
            border: none;
            padding: 3px;
            display: block;
            border-radius: 5px;
            text-align: center;
            font-size: 10px;
            line-height: 15px;
            color: #515151;
            font-weight: 700;
            max-width: 75px;
            max-height: 57px;
            text-decoration: none;
        }

        .title-tourh {
            display: flex;
            color: #0031b0;
            margin: 50px auto;
            padding-bottom: 10px;
            border-bottom: 1px solid #eee;
            width: 100%;
        }

        .sub_main {
            margin-bottom: 20px;
        }



        .title_main {
            margin-bottom: 30px;
            position: relative;
            border-right: 2px #012a93;
            margin-top: 20px;
            text-align: center;
        }

        .title_main span {
            display: inline-block;
            vertical-align: top;
            display: inline-block;
            color: #fff;
            font-weight: 600;
            text-transform: uppercase;
            line-height: 47px;
            height: 47px;
            font-size: 16px;
            background: #012a93;
            padding-left: 70px;
            padding-right: 45px;
            position: relative;
        }

        .thumbnail img {
            margin-right: 0%;
        }



        @media only screen and (max-width: 768px) {
            .navbar {
                flex-direction: column;
            }

            .navbar a {
                padding: 5px;
                /* Giảm khoảng cách giữa các liên kết trên thanh điều hướng */
            }

            .navbar-logo img {
                width: 100px;
                /* Giảm kích thước của logo */
            }

            .product-info {
                flex-direction: column;
            }

            .row {
                flex-direction: column;
            }

            .main {
                flex-direction: column;
            }

            .product img {
                max-width: 100%;
                /* Đảm bảo hình ảnh không vượt quá kích thước của màn hình */
            }


        }
    </style>
</head>

<body>

    <!-- Thanh điều hướng -->
    <div class="navbar">
        <a href="#home">Trang chủ</a>
        <a href="gioithieu.html">Giới thiệu</a>
        <a href="#contact">Liên hệ</a>
        <!-- Thanh tìm kiếm -->
        <div class="search-container">
            <form action="/search" method="get">
                <input type="text" placeholder="Tìm kiếm..." name="search">
                <button type="submit">Tìm kiếm</button>
            </form>
        </div>
        <div class="navbar-logo">
            <img src="images/zyro-image (1).png" alt="Logo">
        </div>
        <div class="tieu-de">
            <p><strong> +(84) 931-855-836<br>
                    Tổng đài tư vấn miễn phí</strong>
            </p>
        </div>
    </div>

    <nav class="navbar navbar-expand-sm bg-light navbar-dark sticky-top ">
        <div class="container-fluid">
            <a class="navbar-brand" href="#">Trọng-Tour</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#collapsibleNavbar">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="collapsibleNavbar">
                <ul class="navbar-nav me-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="">
                            <i class="fas fa-home"></i> Khách Sạn
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">
                            <i class="fas fa-luggage-cart"></i> Tour
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">
                            <i class="fas fa-phone"></i> Vé Máy Bay
                        </a>
                    </li>
                </ul>
                <ul class="navbar-nav me-2">
                    <li class="nav-item">
                        <a class="nav-link" href="dangnhap.html">
                            <i class="fas fa-sign-in-alt"></i> Đăng Nhập
                        </a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">
                            <i class="fas fa-american-sign-language-interpreting"></i> Đăng Kí
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Ảnh bìa của trang web -->
    <!-- Carousel -->
    <div id="demo" class="carousel slide" data-bs-ride="carousel">

        <!-- Indicators/dots -->
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#demo" data-bs-slide-to="0" class="active"></button>
            <button type="button" data-bs-target="#demo" data-bs-slide-to="1"></button>
            <button type="button" data-bs-target="#demo" data-bs-slide-to="2"></button>
        </div>

        <!-- The slideshow/carousel -->
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="images/shutterstock1169930359-1593591-8866-7555-1593591174.jpg" alt="" class="w-100">
            </div>
            <div class="carousel-item">
                <img src="images/Khach-san-duong-Vo-Nguyen-Giap-ĐN-02.jpg" alt="" class="w-100">
            </div>
            <div class="carousel-item">
                <img src="images/slide4.jpg" alt="" class="w-100">
            </div>
        </div>

        <!-- Left and right controls/icons -->
        <button class="carousel-control-prev" type="button" data-bs-target="#demo" data-bs-slide="prev">
            <span class="carousel-control-prev-icon"></span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#demo" data-bs-slide="next">
            <span class="carousel-control-next-icon"></span>
        </button>
        <hr>
        <div class="row">
            <div class="side">
                <h2>Vị trí </h2>
                <img src="images/picture1-1639233879575839620435.jpg" style="max-width: 100%; height: auto;">
                <p><Strong>Đà Nẵng là một thành phố lớn tại Việt Nam, nằm ở miền Trung của đất nước này..</Strong></p>
                <h3>Danh sách xe dịch vụ </h3>
                <img src="images/grab-hyundai1.webp">
                <h3>Grab</h3>
                <img src="images/6-taxi-xanh-sm-16868906422141212552685.webp">
                <h3>Sanh SM</h3>
                <img src="images/3005554-b771a2430d48d880609d4aab14a0c031.jpg">
                <h3>Mai Linh</h3>
                <h4>Follow Me</h4>
                <p>Facebook</p>
                <p>Youtube</p>
            </div>
            <div class="main">
                <div class="main-content">
                    <h2>Địa Điểm Du Lịch Đà Nẵng Nổi Tiếng Cập Nhật Mới</h2>
                    <div class="product">
                        <div class="product-info">
                            <img src="images/ut8upfi8ui84df7anxdl.webp" alt="Sách 1">
                            <p> Nằm ở độ cao 1.487 mét so với mực nước biển, khu du lịch Bà Nà Hills mở ra “khung trời
                                Châu Âu giữa lòng phố thị”. Nơi đây là điểm đến yêu thích của các tín đồ Instagram, khi
                                quy tụ hàng loạt toạ độ sống ảo đẹp lung linh. Kể “sương sương” thôi thì đã có Cầu Vàng,
                                công trình từng được Tạp chí Time bình chọn là 1 trong 100 điểm đến hàng đầu thế giới,
                                Làng Pháp, Vườn Hoa Le Jardin D’Amour, Bảo Tàng Tượng Sáp và Hầm Rượu Debay. Không thể
                                không nhắc khoảnh khắc “chill cực” khi được lướt giữa mây màn trên tuyến cáp treo dài
                                nhất thế giới, hướng tầm mắt về khung cảnh hùng vỹ của núi Chúa. </p>
                        </div>
                        </p>
                        <h3>1. Bà Nà Hills - Địa Điểm Du Lịch Đà Nẵng Được Yêu Thích</h3>
                        <p>Giá: 100,000 VND</p>
                        <hr>
                        <div class="product-info">
                            <img src="images/ban-dao-son-tra-3-1024x550.webp" alt="Sách 1">
                            <p>Chùa Linh Ứng trên Bãi Bụt, Bán Đảo Sơn Trà cũng là địa điểm du lịch Đà Nẵng rất đáng cân
                                nhắc. Đây là công trình mới với quy mô lớn nhất trong loạt Chùa Linh Ứng trứ danh Đà
                                Thành.
                                Bạn có thể mục sở thị tượng Bồ Tát Quán Thế Âm cao 67 mét - được UNESCO công nhận là
                                tượng
                                Quán Thế Âm cao nhất Đông Nam Á. Từ Chùa Linh Ứng Bãi Bụt, #teamKlook sẽ không khỏi ố á
                                khi
                                chiêm ngưỡng thành phố Đà Nẵng nhộn nhịp song hành bên bãi biển Mỹ Khê lấp lánh nắng
                                vàng.Còn có biệt danh “nàng tiên xanh”, rộng đến 3.439 héc-ta - sở hữu khí hậu quanh năm
                                mát mẻ và hệ sinh thái động thực vật đa dạng bậc nhất Đà Nẵng
                            </p>
                        </div>
                        </p>

                        <h3>Bán Đảo Sơn Trà</h3>
                        <p>Giá: 100,000 VND</p>
                        <hr>
                        <div class="product-info">
                            <img src="images/cam-nang-chi-tiet-kinh-nghiem-du-lich-ngu-hanh-son-tu-a-z-202107131132452614.jpg"
                                alt="Sách 1">
                            <p>Thuỷ Sơn, Kim Sơn, Hoả Sơn, Mộc Sơn và Thổ Sơn là năm núi đá vôi tạo thành Ngũ Hành Sơn -
                                địa điểm du lịch Đà Nẵng “gây thương nhớ” bằng thành vách đá sừng sững, hang động huyền
                                bí cùng quần thể đền chùa cổ kính. Sở hữu thảm xanh thiên nhiên đa tầng, thời tiết ở Ngũ
                                Hành Sơn trong trẻo và mát lành - rất phù hợp cho #teamKlook muốn thưởng ngoạn cảnh đẹp,
                                tạm thời “chạy trốn” khỏi nhịp sống thành thị xô bồ. Khá đông du khách đến Ngũ Hành Sơn
                                là để sưu tầm nhiều tác phẩm nghệ thuật duy mỹ ở Làng Điêu Khắc Đá Mỹ Nghệ Non Nước -
                                làng nghề truyền thống lâu đời hơn 400 năm tuổi tại Đà Nẵng. </p>
                        </div>
                        <h3>Ngũ Hành Sơn</h3>
                        <p> <Strong>Giá: 40.000VND/vé</Strong></p>
                        <hr>
                        <div class="product-info">
                            <img src="images/wem3mrevw9wzbuhejdas.webp" alt="Sách 1">
                            <p>Nằm ở số 119, đường Trần Phú, quận Hải Châu, Chợ Hàn được ví như thánh địa mua sắm khi
                                thoả mãn cả ba tiêu chí: hàng hoá đa dạng, giá thành rẻ và chất lượng xịn sò. Chia thành
                                36 ki-ốt và gần 600 gian hàng, dường như du khách có thể “mang cả thế giới về nhà” từ
                                Chợ Hàn - dù là nhu yếu phẩm, quần áo, quà lưu niệm hay . Tín đồ ăn uống tha hồ lấp đầy
                                chiếc bụng đói với nào là mỳ Quảng, bánh xèo, ốc hút, bánh bèo, chả bò, khô hay mắm cá
                                biển. Đừng ngần ngại trả giá xuống 40% - 50% khi mua sắm để không bị “hớ”, #teamKlook
                                nhé!
                            </p>
                        </div>
                        </p>

                        <h3>Chợ Hàn</h3>
                        <p>Giá: 100,000 VND</p>
                        <hr>
                        <div class="product-info">
                            <img src="images/lzpjwxqxsq0ett4mdfqn.webp" alt="Sách 1">
                            <p>Bạn cho rằng phải đến tận nước Nhật xa xôi thì mới được tận hưởng Osen - a.k.a trải
                                nghiệm tắm suối khoáng nóng xịn sò? Nhầm hơi bị to rồi đấy. Trải rộng hơn 60 héc-ta giữa
                                đồng núi trập trùng và rừng nguyên sinh trù phú, Công Viên Suối Khoáng Nóng Núi Thần Tài
                                chính là “nhà chung” của loạt hồ nước châm cứu, hang động chữa lành, hệ thống suối thiên
                                nhiên bao gồm cả suối nước nóng dồi dào khoáng chất. #teamKlook nhỏ tuổi chắc chắn sẽ mê
                                mệt rạp chiếu phim 9D, 12D cùng công viên nước muôn màu muôn vẻ tại đây.Chẳng còn nghi
                                ngờ gì nữa, đích thị là địa điểm du lịch Đà Nẵng trên cả tuyệt vời dành cho người đi du
                                lịch cùng bạn bè, gia đình. Đặt vé trên Klook để nhận liền tay ưu đãi độc quyền.

                            </p>
                        </div>
                        </p>

                        <h3>Chợ Hàn</h3>
                        <p>Giá: 100,000 VND</p>

                    </div>
                </div>
            </div>

        </div>
    </div>
    <div class="title_main"><span>Khách Sạn - Khu Nghỉ Dưỡng </span></div>
    <div class="container-fluid mt-2">
        <div class="row">
            <div class="col-md-4 text-center">
                <div class="thumbnail">
                    <img src="images/anh5-15263076583301991908567.png" alt="" style="width:100%">
                    <h3 class="text-success">Danang Golden Bay </h3>
                    <h4 class="text-danger"> <span>7.711.407&nbsp;₫</span>
                    </h4>
                    <button class="btn btn-danger"> Đặt Phòng </button>
                </div>
            </div>
            <div class="col-md-4 text-center">
                <div class="thumbnail">
                    <img src="images/caption.jpg" alt="" style="width:100%">
                    <h3 class="text-success">MELIA DANANG BEACH RESORT</h3>
                    <h4 class="text-danger"> <span>7.711.407&nbsp;₫</span></h4>
                    <button class="btn btn-danger"> Đặt Phòng </button>
                </div>
            </div>
            <div class="col-md-4 text-center">
                <div class="thumbnail">
                    <img src="images/view-noi-khu-InterContinental-Danang-Sun-Peninsula.jpg" alt="" style="width:100%">
                    <h3 class="text-success">TInterContinental Danang</h3>
                    <h4 class="text-danger"><span>7.711.407&nbsp;₫</span> </h4>
                    <button class="btn btn-danger">Đặt Phòng </button>
                </div>
            </div>
        </div>
    </div>

    <div class="container-fluid mt-2">
        <div class="row">
            <div class="col-md-4 text-center">
                <div class="thumbnail">
                    <img src="images/khach-san-mikazuki-danang-vietnam-1.jpg" alt="" style="width:100%"">
                    <h3 class=" text-success">Mikazuki Japanese Resorts</h3>
                    <h4 class="text-danger"><span>7.711.407&nbsp;₫</span></h4>
                    <button class="btn btn-danger"> Đặt Phòng </button>
                </div>
            </div>
            <div class="col-md-4 text-center">
                <div class="thumbnail">
                    <img src="images/495550115.jpg" alt="" style="width:100%">
                    <h3 class="text-success">Four Points by Sheraton Danang</h3>
                    <h4 class="text-danger"> <span>7.711.407&nbsp;₫</span> </h4>
                    <button class="btn btn-danger"> Đặt Phòng </button>
                </div>
            </div>
            <div class="col-md-4 text-center">
                <div class="thumbnail">
                    <img src="images/356950307.jpg" alt="" style="width:100%">
                    <h3 class="text-success">Risemount Premier Resort</h3>
                    <h4 class="text-danger"> <span>7.711.407&nbsp;₫</span></h4>
                    <button class="btn btn-danger"> Đặt Phòng </button>
                </div>
            </div>
        </div>
    </div>

    <div class="chat-nav">
        <ul>
            <li> <a href="">
                    <i class="ticon-zalo-circle2"></i>Chat Zalo </a></li>
            <li><a href="">
                    <i class="fas fa-phone"> </i> gọi điện </a></li>
            <li> <a href=""> <i class="fab fa-facebook-messenger"></i> Messenger </a>
            </li>
            <li> <a href="" class=" chat_animation"> <i class="fas fa-envelope"></i> Nhắn tin SMS </a></li>
            <li> <a href=""> <i class="fas fa-map-marker-alt"></i>Tìm đường </a></li>
        </ul>
    </div>
    <div class="title-tourh">
        <h2><i class="fas fa-comment"></i> Ý kiến khách hàng</h2>
    </div>
    <span style="vertical-align: bottom; width: 50%; height: 215px;"><iframe name="fcb1fa8e1a77519ed" width="800px"
            height="100px" data-testid="fb:comments Facebook Social Plugin" title="fb:comments Facebook Social Plugin"
            frameborder="0" allowtransparency="true" allowfullscreen="true" scrolling="no" allow="encrypted-media"
            src="https://www.facebook.com/v2.10/plugins/comments.php?app_id=&amp;channel=https%3A%2F%2Fstaticxx.facebook.com%2Fx%2Fconnect%2Fxd_arbiter%2F%3Fversion%3D46%23cb%3Df84ba734c181f11f4%26domain%3Ddulichmaitravel.vn%26is_canvas%3Dfalse%26origin%3Dhttps%253A%252F%252Fdulichmaitravel.vn%252Ff66cda02d27abe9b4%26relation%3Dparent.parent&amp;container_width=930&amp;height=100&amp;href=https%3A%2F%2Fdulichmaitravel.vn%2Ftour-mien-trung-4n3d-da-nang-hoi-an-ba-na-hue-phong-nha-di-san-mien-trung&amp;locale=vi_VN&amp;numposts=5&amp;sdk=joey&amp;version=v2.10&amp;width="
            style="margin-right: auto;border: none; visibility: visible; width: 80%; height: 215px;"
            class=""></iframe></span>
    <hr>
    <footer class="footer text-center">
        <div class="container">
            <span>&copy; 2024 Trọng-Tour. All rights reserved.</span>
            <span class="float-end">Designed with <i class="fas fa-heart"></i> by Your Name</span>
        </div>
    </footer>

</body>

</html>
