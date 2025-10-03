# Product Rating System Setup Guide

## 🚀 What's Been Fixed

### 1. **Color Change Functionality** ✅
- Color buttons now properly switch product images when clicked
- Active state is maintained for selected colors
- Hover effects work correctly

### 2. **Rating System** ✅
- Star rating system is fully functional
- Ratings are stored in the database
- Average ratings are calculated and displayed
- Guest users can also rate products

## 📋 Database Setup Required

### Step 1: Run the SQL Setup
Execute the SQL commands in `database_setup_ratings.sql` in your database:

```sql
-- This will create the required tables and columns
-- Run this in phpMyAdmin or your MySQL client
```

### Step 2: Verify Table Creation
After running the SQL, you should have:
- `product_ratings` table (new)
- `avg_rating` and `total_ratings` columns in your `products` table

## 🔧 How It Works

### Color System
1. **Click any color button** → Product image changes immediately
2. **Hover over product** → Shows back image
3. **Active color** → Highlighted with border

### Rating System
1. **Click stars** → Rating is saved to database
2. **Guest users** → Can rate products (stored with unique guest ID)
3. **Logged users** → Ratings linked to their account
4. **Average display** → Shows current average rating and total count

## 📁 Files Created/Modified

### New Files:
- `save-product-rating.php` - Handles saving ratings
- `get-product-rating.php` - Retrieves existing ratings
- `database_setup_ratings.sql` - Database setup script
- `RATING_SETUP_GUIDE.md` - This guide

### Modified Files:
- `index.php` - Enhanced color and rating functionality

## 🎯 Features

### Color Selection
- ✅ Real-time image switching
- ✅ Active state management
- ✅ Hover effects preserved
- ✅ Responsive design

### Rating System
- ✅ 1-5 star rating
- ✅ Database storage
- ✅ Average calculation
- ✅ Guest user support
- ✅ User rating history
- ✅ Real-time updates

## 🚨 Important Notes

1. **Database Required**: Must run the SQL setup first
2. **Guest Users**: Can rate products without accounts
3. **One Rating Per User**: Users can only rate each product once (can update)
4. **Performance**: Indexes added for better query performance

## 🧪 Testing

1. **Color Change**: Click different color buttons on any product
2. **Rating**: Click on stars to rate products
3. **Database**: Check `product_ratings` table for stored ratings
4. **Average**: Verify average ratings update in `products` table

## 🔍 Troubleshooting

### Color not changing?
- Check browser console for JavaScript errors
- Verify image paths in database

### Rating not saving?
- Check if database tables exist
- Verify file permissions for PHP files
- Check browser console for fetch errors

### Database errors?
- Ensure MySQL version supports `IF NOT EXISTS`
- Check database connection in `connection.php`

## 📞 Support

If you encounter issues:
1. Check browser console for errors
2. Verify database setup completed
3. Check file permissions
4. Ensure all files are in correct locations

---

**Your rating system is now fully functional!** 🎉
