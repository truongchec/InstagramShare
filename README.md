# InstageamShare
Insgram Share&amp;Download
# How to Code:-

Get Url from Instagram
Use InstagramApi to get the final url of image and video
or You can get into source code using JSoup Library Jsoup Maven and Gradle Dependencies
Once You get the Final Image/Video Url Use Picasso or Glide Library to Load images from url Glide Github
For Loading video from url get Url connection
try {
     	URL myUrl = new URL(url);
      	URLConnection connection = myUrl.openConnection();      
      	is = connection.getInputStream();
      	bis = new BufferedInputStream(is);
      	fos = new FileOutputStream(destFile); 
	int current = 0;
   	while ((current = bis.read()) != -1) {
        	fos.write(current);
         }
        fos.close();
    }catch(Exception e) {
      //Log.e(TAG, "Error while downloading and saving file !", e);
    }
For Printing Image Use below piece of code
private void doPhotoPrint() {
    PrintHelper photoPrinter = new PrintHelper(getActivity());
    photoPrinter.setScaleMode(PrintHelper.SCALE_MODE_FIT);
    Bitmap bitmap = BitmapFactory.decodeResource(getResources(),R.drawable.droids);
    photoPrinter.printBitmap("droids.jpg - test print", bitmap);
}
© 2020 GitHub, Inc.
