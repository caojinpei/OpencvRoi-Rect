#include "cv.h"
#include "highgui.h"

using namespace cv;

void main()
{
	Mat image = imread("C:\\Users\\Leo\\Desktop\\lena.jpg");
	Rect rect1(256, 256, 128, 128);
	Rect rect2(224, 224, 128, 128);

	Mat roi1;
	image(rect1).copyTo(roi1);
	imshow("1", roi1);
	waitKey(0);

	Mat roi2;
	image(rect2).copyTo(roi2);
	imshow("2", roi2);
	waitKey(0);

	cv::Rect rect3 = rect1&rect2;
	Mat roi3;
	image(rect3).copyTo(roi3);
	imshow("3", roi3);
	waitKey(0);

	Rect rect4 = rect1|rect2;
	Mat roi4;
	image(rect4).copyTo(roi4);
	imshow("4", roi4);
	waitKey(0);

	Rect rect5(10, 10, 128, 128);
	roi1.copyTo(image(rect5));
	imshow("5", image);
	waitKey(0);
}
