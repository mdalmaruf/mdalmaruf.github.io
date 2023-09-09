<style>
  .gallery {
    display: flex;
    flex-wrap: wrap;
    gap: 16px;
  }
  .gallery-item {
    position: relative;
    border: 2px solid #000;
    border-radius: 12px;
    overflow: hidden;
    width: 200px;
  }
  .gallery-item img {
    display: block;
    max-width: 100%;
  }
  .gallery-item-label {
    position: absolute;
    bottom: 0;
    background: rgba(0, 0, 0, 0.5);
    color: #fff;
    width: 100%;
    text-align: center;
    padding: 8px;
    box-sizing: border-box;
    border-radius: 0 0 10px 10px;
    font-size: 14px;
  }
</style>

<div class="gallery">
  <div class="gallery-item">
    <img src="https://picsum.photos/seed/picsum/200/300" alt="Image 1">
    <div class="gallery-item-label">Date: 01/01/2023<br>Location: New York<br>Event: Wedding</div>
  </div>
  <div class="gallery-item">
    <img src="https://picsum.photos/seed/picsum/200/300" alt="Image 2">
    <div class="gallery-item-label">Date: 02/02/2023<br>Location: Los Angeles<br>Event: Birthday Party</div>
  </div>
  <div class="gallery-item">
    <img src="https://picsum.photos/seed/picsum/200/300" alt="Image 3">
    <div class="gallery-item-label">Date: 03/03/2023<br>Location: San Francisco<br>Event: Corporate Event</div>
  </div>
  <div class="gallery-item">
    <img src="https://picsum.photos/seed/picsum/200/300" alt="Image 4">
    <div class="gallery-item-label">Date: 04/04/2023<br>Location: Miami<br>Event: Anniversary</div>
  </div>
</div>
